# DiceTask1

####Make docker file

nano dockerfile
FROM ubuntu:latest OR FROM ubuntu:alpine
WORKDIR /app
ADD . /app ####(. current directory)
RUN apt update && apt install Nginx -y
Copy ./index.html /var/log/html 
CMD ["service","nginx","start"]
LABEL color=red

###Build Docker File
sudo docker build -t ibrarimage . (. current directory)


#Push image
docker login (docker hub)
docker push dockerhubname/imagename

#########Git commands
git init
git add README.md
git commit -m "first commit"
git branch -M main
git remote add origin https://github.com/ibrar-cloud/DiceTask1.git
git push -u origin main

nano index.html (code file)
git init (initialize)
git add index.html  (stagging)
git status (check status)
git commit -m"message" (commmit/local directory)
Make repository on Github
git remote add origin https://github.com/ibrar-cloud/DiceTask1.git (github add to origin)
git push origin master  (push on github)

#####Dice Task 2

sudo docker run -it -d --name -p 80:80 ubuntu (p publish , 1st 80 host , 2nd 80 container)
#check Images
sudo docker images

#Check status
sudo systemctl status docker

#Start Docker
sudo systemctl start docker

#Stop Docker
sudo systemctl stop docker

#Check Version
sudo docker -v

#Docker Run
sudo docker run -it -d ubuntu
sudo docker run -it -d --name ubuntu
sudo docker run -it -d --ibrar -p 80:80 ubuntu (p publish , 1st 80 host , 2nd 80 container)


#Check Docke process
sudo docker ps -a
sudo docker ps 

#Container stop start restart remove and kill
sudo docker restart name/id
sudo docker stop name/id
sudo docker start name/id
sudo docker rmi name/id
sudo docker rm name/id
sudo docker kill name/id


#Inter in container
sudo docker exec -ti ibrar bash
