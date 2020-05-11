# Flask_aws_EC2

Basic deployment of flask application on EC2 instance with Docker.

# How to run

- Run pip install -r requirements.txt
- sudo docker-compose up --build -d

# steps to follow

1- ssh -i flask.pem ubuntu@**IP ADDRESS**<br>
2-Once in instance, add dependencies: <br>

sudo apt-get update <br>
docker (to check if we have docker installed)

3- clone git by:<br>

git clone (url)

4-Install docker using: <br>

sudo apt-get install docker-compose

