DOCUMENTATION


Step 1: launch the server 
Then connect in mobaextrem
And ssh it
Install docker 
cat ss.sh
# Add Docker's official GPG key:
sudo apt-get update
sudo apt-get install ca-certificates curl
sudo install -m 0755 -d /etc/apt/keyrings
sudo curl -fsSL https://download.docker.com/linux/ubuntu/gpg -o /etc/apt/keyrings/docker.asc
sudo chmod a+r /etc/apt/keyrings/docker.asc

# Add the repository to Apt sources:
echo \
  "deb [arch=$(dpkg --print-architecture) signed-by=/etc/apt/keyrings/docker.asc] https://download.docker.com/linux/ubuntu \
  $(. /etc/os-release && echo "$VERSION_CODENAME") stable" | \
  sudo tee /etc/apt/sources.list.d/docker.list > /dev/null
sudo apt-get update

And clone both frontend and backend repos
git clone  https://github.com/Anand-1432/Techdome-frontend.git

git clone https://github.com/Anand-1432/Techdome-backend.git

Step 2 : create docker file for both frontend and backend
For frontend 
![0](https://github.com/user-attachments/assets/c293ab60-4b70-4799-a711-03eb4aa5edb7)

Build and run it
sudo apt-get install docker-ce docker-ce-cli containerd.io docker-buildx-plugin docker-compose-plugin
   45  sudo docker run hello-world
   46  docker build -t react-nginx .
   47  sudo usermod -aG docker $USER
   48  docker build -t react-nginx .
   49  sudo docker build -t react-nginx .
   50  docker run -d -p 80:80 react-nginx
   51  sudo docker run -d -p 80:80 react-nginx

For backend
![1](https://github.com/user-attachments/assets/1e4ca4bf-e650-47cc-b61d-cf6fa8566d9a)
Same for this
  docker build -t backend-app1 .
   78  docker ps
   79  docker ps -a
   80  docker rm -f 40 fa 73
   81  docker ps
   82  docker run -p 3000:3000 backend-app
   83  docker run -d -p 3000:3000 backend-app1





Step 3 : create dozzle for monitoring for frontend and backend
For frontend
![2](https://github.com/user-attachments/assets/7b253486-156c-4085-9b03-40ae60dc7d51)

For backend
![3](https://github.com/user-attachments/assets/24733daa-0da3-4643-abbf-8e08828869ff)

Command for this 
sudo docker images  108  docker ps
  109  docker run -d -v /var/run/docker.sock:/var/run/docker.sock -p 8080:8080 amir20/dozzle:latest
  110  sudo docker ps

Step 4 : check the deployment
![4](https://github.com/user-attachments/assets/0be92cf1-7227-4be7-abe1-2321bbf54f12)
Step 5 : now push this all to github
  git remote add origin https://github.com/mathematicsgk/Tech_dome-.git
  188  git remote -v
  189  git init
  190  git add .
  191  git push
  192  git push origin main
  193  git pull origin main
  194  git add .
  195  git commit -m "add"
  196  git push origin main
  197  git pull origin main --rebase
  198  git branch
  199  git checkout main
  200  git add README.md
  201  git rebase --continue
  202  git push origin main --force

Issues faced

Method1: In System:windows
Firstly I tried docker software and minkube software in my system so out of 3 containers two container is created but one is running and another is completed and got error in port service.
![5](https://github.com/user-attachments/assets/79e465ac-0b38-4cea-9ada-a4f166e727d6)
 
![6](https://github.com/user-attachments/assets/d8f51715-1470-4c97-aebf-26bc5a92c619)

![7](https://github.com/user-attachments/assets/ab80db99-cc24-4766-945d-68e3290ff1b2)

Method2: Via Azure Virtual Machine 
Frontend not connecting backend due to database connectivity issue.


Remark:
Source of learning and deployment done via google and online.And I am new learner in devops but I know about Azure services and Ethical hacking ,iot and cybersecurity and I try my best .And my semester exam running so that’s why I am late.

Thanksyou


