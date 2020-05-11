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

```
(to check if we have docker installed)
3- clone git by:<br>



```bash

git clone (url)

```

4-Install docker using: <br>



```bash

sudo apt-get install docker-compose

```

5- check again docker image: <br>



```bash

docker <br>

docker-compose 

```

6- Install pip : <br>


```bash

sudo apt install python3-pip

```

7- Run requirements.txt : <br>

```bash

pip3 install -r requirements.txt

```

8- Check if all needed dependencies are there<br>

```bash

pip3 freeze

```
9-Check if we have docker images:<br>

```bash

sudo docker images

```
10-Build docker image : <br>


```bash

sudo docker-compose build

```

11-check again docker images : <br>

```bash

sudo docker images

```

12-To run this image:<br>

```bash

sudo docker-compose up --build -d

```

13-Remember to open ports from "Security Groups":<br>

```bash

port 8000, 8080 
```

On a side note, we can use vim editor by using<br>

```bash

sudo vim fliename
```
