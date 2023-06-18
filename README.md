# guvi_task7!

**Create a custom docker image for nginx and deploy it using docker-compose, where the volume mount should be at /var/opt/nginx location. Push the created custom docker image to your docker hub.**

![task7 1](https://github.com/suganyaanbalagan123/guvi_task7/assets/133192593/bd23d704-5a58-4fcf-b382-a65633b29490)

![Task 7 2](https://github.com/suganyaanbalagan123/guvi_task7/assets/133192593/2d1092ae-7655-4023-b78d-9e1a829c9613)

**The image is running in the prot 2000**

![7 3](https://github.com/suganyaanbalagan123/guvi_task7/assets/133192593/311857f0-a844-4569-baf1-af4d79a73814)

**The container is running in the port 1000**

![7 4](https://github.com/suganyaanbalagan123/guvi_task7/assets/133192593/0aeeba18-65ce-4e1e-a0af-910613d6f111)

**2.pushing the created docker ngnix image to docker hub
**

![task77](https://github.com/suganyaanbalagan123/guvi_task7/assets/133192593/aa05ac4d-a509-415f-8d1b-fb1ed5f8178d)

**3.pushed image in my dockerhub repo**

![task7 4](https://github.com/suganyaanbalagan123/guvi_task7/assets/133192593/6745b1a2-617b-4ebc-8ac6-3d70728e8031)


**Docker comments**

    2  sudo apt update
    3  sudo apt install docker.io
    4  sudo apt install git
    5  mkdir ngnix
    6  cd ngnix
    7  vi index.html
    8  vi Dockerfile
    9  pwd
   10  vi Dockerfile
   11  vi docker-compose.yml
   12  sudo docker build -t ngnix .
   13  docker images
   14  sudo docker images
   15  sudo docker run -d --name my_nignix_container  -p 8080:80 ngnix
   16  curl localhost:8080
   17  vi Dockerfile
   18  sudo docker build -t ngnix .
   19  sudo docker images
   20  sudo docker run -d --name my_nignix_container  -p 3000:80 ngnix
   21  sudo docker run -d --name my_nignix_container  -p 1000:80 ngnix
  103  sudo docker build -t ngnix_image .
  104  sudo docker run -d -p 3000:80 ngnix_image
  105  sudo docker run -d -p 2000:80 ngnix_image
  106  vi docker-compose.yml
  107  sudo docker-compose up
  205  sudo docker login -u "suganyamadhan1996" -p "Suman#123" docker.io
  220  sudo docker tag ngnix-html:latest suganyamadhan1996/ngnix1:myfirstpush-ngnix 
  221  sudo docker push suganyamadhan1996/ngnix1:myfirstpush-ngnix
  222  history
