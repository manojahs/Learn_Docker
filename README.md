# Learn_Docker

What is the challege?  
Code works in my machine not in other machine to resolve this issue we use Docker Container

Basically its Packaging solution to simplify the deployment (it contains like code, solution, instruction, operatinig system everything which need to run your application that is being stored in the container same container works in local machine and once u put into server it will works there too)


1)Container are built on top of Images.  
2)Containers are created using images.  
3)Image which containes like dot net applicaton executable files to run the dot net app.  
4)For using the nodejs/sql/dotnet app for any application run in docker we have a special application called docker hub where we will get all the programming languages as Images  
5)Docker Images are standalone executable files which is used to create a container. and docker images are sharable and portable  

Images
---------
Images of docker build by Layers 

<img width="916" alt="image" src="https://github.com/user-attachments/assets/fca352c6-461b-496c-bac4-09d3182040d3" />  

To run the dot net application we need to create several layers and finally we need to put Final Layer inside the container  

<img width="865" alt="image" src="https://github.com/user-attachments/assets/8a015b8b-0bf8-4662-b7a4-4939854fb609" />  

Docker vs VM
------------------

<img width="920" alt="image" src="https://github.com/user-attachments/assets/2efe7ea4-c785-4e87-ae62-9b31d35a283e" />  

Each VM containes its own OS so which will make heavier so in docker container for each container we will be not having seperate OS for each thats why it will be Lightweight.  

Containers takes less memory when compare to VM  

Search this and click on sdk copy the command paste it in cmd prompt  
https://hub.docker.com/r/microsoft/dotnet  

To get the id of all the container and to remove all the container
----------------------------------  
$(docker ps -a -q)  
To remove all the container: docker rm $(docker ps -a -q)  

To get the id of all the images and to remove all the images  
-------------------------------------
docker images -q
docker rmi $(docker images -q)  








