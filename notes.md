ps -ef | grep jenkins
then open the enbound rule or port in the instance of 8080 for the jenkins
> install suggested plugins
sudo apt-get install docker.io
sudo su -
usermod -aG docker jenkins
usermod -aG docker ubuntu
sudo systemctl restart docker
su - jenkins
docker run hello-world
 explian ci/cd process  ? 
how can you handle worker node in the cluster when it is down ?
how the jennkins works 
what is kubernetes , pods , and services ?
 

 if you want to make a simple react app then 1st dwnld node then go to terminal  
 node -v 
 npx create-react-app testapp
 cd testapp
 npm start 

remove node_modules from the folder

if you want dockerfile then in this folder (testapp) create a file named Dockerfile
inside this 
FROM node:latest   (we can give any version)

WORKDIR /myapp
COPY . /myapp (this will copy all files of dir to myapp)
EXPOSE 3000 (we can give any port)
RUN npm install
CMD ["npm" , "start"]


then build and image for this dockerfile 
docker build -t <imagename> .
docker run -d -p 3000:3000 --name <containernaem> <imagename>

docker ps
docker stop <containername>
interactive mode (-it)


 
bind the mount point 
-v <path of physical point>:</mount point> (/myapp/server.txt) 
persistent container 
create volume to persist the point 




