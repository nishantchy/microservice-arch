# Microservice Application

This project is only based on understanding how microservice applications works. It is created using python Flask.

## Initialize Project in virtual environment in auth. Inside `/microservice-arch/python/src/auth/` run command:

```bash
python -m venv venv
```

## Run the virtual environment in gitbash terminal using:

```bash
source venv/Scripts/activate
```

## Inorder to access database, use command:

```bash
winpty mysql -u root -p
```

or just

```bash
mysql -u root -p
```

- Authentication service
  Authentication service uses MySQL database with user specified in init.sql file.
  Inorder to check the file and modify it run cmd inside `/microservice-arch/python/src/auth/`

```bash
  mysql -uroot -p < init.sql
```

## Run Auth Service using command:

```bash
python server.py
```

## Build the docker image using command:

```bash
docker build . -t auth-micro-service
```

## Tag the docker image using command:

```bash
docker tag <image_id> <your_username>/auth-micro-service:tagname
```

## Push the image to your dockerhub repository:

```bash
docker push <your_username>/auth-micro-service:tagname
```

--1:07
