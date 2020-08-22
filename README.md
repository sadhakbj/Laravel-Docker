# Laravel LEMP Docker

Docker development implementation for Laravel 7.\* with:

- Nginx
- MySql
- PHP7.4
- Redis
- Node

## Installation

- Clone this repository: `git clone git@github.com:sadhakbj/Laravel-Docker.git`
- Make sure you have docker installed on your local machine, you do not need to have php / mysql / redis / node installed on your machine
- Set the environment variables in `.env` file
- Run command: `docker-compose up --build -d`
- You can access the project at: `http://localhost:8000`
- Running migrations: `docker-compose run --rm artisan migrate` or `make migrate`
- Running composer install: `docker-compose run --rm composer install` or `make composer-install`

### Run php / other service on bash mode

- `docker exec -it php /bin/sh`

### Special credits:

- [Andrew Schmelyun](https://www.youtube.com/channel/UCc07-IBVwRlOsMg2WMdd8Sg) for his videos on docker for Laravel.
