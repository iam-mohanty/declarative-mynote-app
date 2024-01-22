# Simple Notes App👍
This is a simple notes app built with React and Django.

## Requirements
1. Python 3.9
2. Node.js
3. React

## Installation
1. Clone the repository
```
git clone https://github.com/kloudskart/declarative-mynote-app.git
```

2. Build the app
```
docker build -t notes-app .
```

3. Run the app
```
docker run -d -p 8000:8000 notes-app:latest
```

## Nginx

Install Nginx reverse proxy to make this application available

`sudo apt-get update`
`sudo apt install nginx`



# jenkins-nodeapp👇😎

# 1. install ubuntu 

create aws ubuntu-22 server , login as : ubuntu 

sudo apt-get update 

sudo apt install docker.io -y 

sudo usermod -aG docker $USER

sudo reboot , again login

# 2. jenkins install

sudo apt install openjdk-17-jre -y

java --version

sudo wget -O /usr/share/keyrings/jenkins-keyring.asc \
  https://pkg.jenkins.io/debian-stable/jenkins.io-2023.key
  
echo deb [signed-by=/usr/share/keyrings/jenkins-keyring.asc] \
  https://pkg.jenkins.io/debian-stable binary/ | sudo tee \
  /etc/apt/sources.list.d/jenkins.list > /dev/null

  
sudo apt-get update

sudo apt-get install jenkins

login jenkins

# 3. start project

create pipeline project

mention anything inside description

github projects : mention ur github repo ; https://github.com/iam-mohanty/docker-compose-jenkins-declarative-nodeapp.git

add syntax in pipeline section (paste it from jenkinsfile) , build

sudo usermod -aG docker jenkins

sudo reboot

again build now

# 4. create docker-hub credential

manage jenkins -> credentials -> goto system -> global credential -> add credential -> mention ur dockerhub username & pw , id : dockerHub

# 5. install docker-compose

sudo apt-get install docker-compose -y

# 6. access app

public-ip:8000
