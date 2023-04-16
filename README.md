# Cinema service API


API service for cinema management written on DRF

### Installing using GitHub

install PostgresSQL and create db

1. Clone the source code:

```bash
git clone https://github.com/Thirteenthskyi/cinema_service.git
cd cinema_service
```
2. Install PostgresSQL and create DB.
3. Install modules and dependencies:

```bash
python -m venv venv
venv\Scripts\activate (on Windows)
source venv/bin/activate (on macOS)
pip install -r requirements.txt
```

4. `.env_sample` 
This is a sample .env file for use in local development.
Duplicate this file as .env in the root of the project
and update the environment variables to match your
desired config. You can use [djecrety.ir](https://djecrety.ir/)

5. Use the command to configure the database and tables:

```bash
python manage.py migrate
```

6. Start the app:

```bash
python manage.py runserver
```

### Run with docker
Docker should be installed

```commandline
docker-compose build
docker-compose up
```

### Getting access
- create user via /api/user/register/
- get access token via /api/user/token/

## Features
- JWT authenticated
- Admin panel /admin/
- Documentations is located at /api/doc/swagger/
- Managing orders and tickets
- Creating movies with genres, actors
- Creating movie sessions
- Filtering movies and movie sessions
