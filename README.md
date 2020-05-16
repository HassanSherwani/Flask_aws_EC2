# Flask_aws_EC2

Basic deployment of flask application on EC2 instance with Docker.


# steps to follow

1- start EC2 instance:<br>
```bash

ssh -i flask.pem ubuntu@IP ADDRESS

```

2-Once in instance, add dependencies: <br>



```bash

sudo apt-get update 

```

```bash

docker

OR 

docker-compose

```
(to check if we have docker installed)
<br>
3- clone git by:<br>



```bash

git clone (url)

```

4-Install docker using: <br>



```bash

sudo apt-get install docker-compose

OR

sudo apt-get install docker-compose -y

```

5- check again docker image: <br>



```bash

docker 

docker-compose 

```

6- Install pip3 : <br>


```bash

sudo apt install python3-pip

```

7- Check if all needed dependencies are there<br>

```bash

pip3 freeze

```

8- Run requirements.txt : <br>

```bash

pip3 install -r requirements.txt

```


9- Install unzip command :<br>

```bash
sudo apt install unzip
```

10-Install gnupg2 pass in case of fargate implementation <br>

```bash
sudo apt install gnupg2 pass
```


11-Check if we have docker images:<br>

```bash

sudo docker images

```
12-Build docker image : <br>


```bash

sudo docker-compose build

```

13-check again docker images : <br>

```bash

sudo docker images

```

14-To run this image:<br>

```bash

sudo docker-compose up --build (for building image for 1st time and running at same time)

OR

sudo docker-compose up --build -d (to run docker image and also keep terminal console in function)

OR 

sudo docker-compose up (only for running docker image)

```
15- Check current running images by:<br>
```bash
sudo docker ps

```
16-Remember to open ports from "Security Groups":<br>

```bash

port 8000, 80
```

17- Associate Elastic IP

18- Setup SSL certificate into your AWS EC2 instance i.e using https with elastic IP

- ^On a side note, we can use vim editor by using<br>

```bash

sudo vim fliename
```
- ^ for deleting docker image: <br>

https://linuxize.com/post/how-to-remove-docker-images-containers-volumes-and-networks/

19- To Install AWS CLI v2 & configure IAM role

curl "https://awscli.amazonaws.com/awscli-exe-linux-x86_64.zip" -o "awscliv2.zip"
