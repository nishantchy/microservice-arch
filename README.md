# Microservice Application

This project is only based on understanding how microservice applications works. It is created using python Flask.

## Initialize Project in virtual environment

```bash
python -m venv venv
```

## Run the virtual environment in gitbash terminal using

```bash
source venv/Scripts/activate
```

## Inorder to access database, use command

```bash
winpty mysql -u root -p
```

- Authentication service
  Authentication service uses MySQL database with user specified in init.sql file.
  Inorder to check the file and modify it run cmd inside `/microservice/python/src/auth/`
  ```bash
  mysql -uroot -p < init.sql
  ```
