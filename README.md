# Braulg **API**

### Looking for main repo?

Read README.md here -> https://github.com/kholostyak17/braulg

## Technologies used in this project:
- [X] Python
- [X] Flask
- [X] PostgreSQL
- [X] alembic
- [X] werkzeug
- [X] JWT
- [X] Cloudinary

## Back-End Manual Installation:

Make sure you have Python 3.8, Pipenv and a database engine (Postgres recomended)

1. Install the python packages: `$ pipenv install`
2. Create a .env file based on the .env.example: `$ cp .env.example .env`
3. Install your database engine and create your database, depending on your database you have to create a DATABASE_URL variable with one of the possible values, make sure you replace the values with your database information:

| Engine    | DATABASE_URL                                        |
| --------- | --------------------------------------------------- |
| SQLite    | sqlite:////test.db                                  |
| MySQL     | mysql://username:password@localhost:port/example    |
| PostgreSQL| postgres://username:password@localhost:5432/example |

4. Migrate the migrations: `$ pipenv run migrate` (skip if you have not made changes to the models on the `./src/api/models.py`)
5. Run the migrations: `$ pipenv run upgrade`
6. Run the application: `$ pipenv run start`