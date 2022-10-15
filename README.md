# College Management System

In the times of covid, when education has totally become digital, there comes a need for a system that can connect
teachers, students, and HOD and that was the motivation behind building this project.

## Setup

- On project initialisation, clone the repository using

```sh
git clone https://github.com/parthjetani/college-management-system.git
```

> _Note:_ This needs to be done only once

- Create .env file in root folder and copy content of env file and fill the values

## (1) Run project using docker

- Install docker and docker-compose in your system
- Now run the commands

```sh
docker-compose build
```

```sh
docker-compse up
```

```sh
docker exec -it <django-container-id> python manage.py createsuperuser
```

Then go to the browser and enter the url http://127.0.0.1:8000/

## (2) Run project using normal django method

Create virtual environment

```sh
python -m venv venv
```

After creating a virtual environment (optional), activate it by running

For windows, activate it this way

```sh
venv/Scripts/activate
```

For other operating system like Linux and MacOS, use

```sh
source venv/bin/activate
```

### (i) Installing project dependencies

To install the project dependencies, use

```sh
pip install -r requirements.txt
```

### (ii) Run the commands makemigrations and migrate

```sh
python manage.py makemigrations
```

```sh
python manage.py migrate
```

### (iii) Create superuser(HOD)

```shell
python manage.py createsuperuser
```

Then go to the browser and enter the url http://127.0.0.1:8000/
