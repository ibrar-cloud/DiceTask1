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
sudo docker run -it -d --name -p 80:80 ubuntu (p publish , 1st 80 host , 2nd 80 container)

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
