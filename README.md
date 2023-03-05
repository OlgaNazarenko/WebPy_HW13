##  WebPy_HW13

For this project it was used poetry, which is designed for dependency management and packaging in this project. It 
allowed declaring the libraries of this project depends on and manages (install/update) them for you. To activate 
the virtual environment, you need to run the command:

      poetry shell

### Part 1:
REST API for storing and managing contacts [^1]. Run the following command to start the FastAPI server in folder *REST*:

      python3 (py) main.py

For this project was done the following:
- verification of the registered user's e-mail;
- added teh limit of requests to the contact routes along with the rate at which contacts are created:
- CORS for your REST API;
- the option to update the user's avatar. For this purpose was used the Cloudinary service;
- all sensitive info is stored in the .env file[^3];
- Docker Compose to run all services and databases in the application (Postgres and Redis):

    docker-compose up


### Part 2:
Django project (created site using Django (similar to http://quotes.toscrape.com))[^2]. Run the following command to start the server in folder *quotes*:

      python3 (py) manage.py runserver

For this project was done the following:
- added a password reset mechanism for a registered user; 
- all environment variables are stored in the .env file and used in the settings.py file


[^1]: Login credentials -> Seoul@example.com
      password -> 123456

[^2]: Login -> Japan, 
      Password -> Seoul2023!

[^3]: POSTGRES_DB=
    POSTGRES_USER=
    POSTGRES_PASSWORD=
    POSTGRES_PORT=
    
    SQLALCHEMY_DATABASE_URL=
    SECRET_KEY_JWT=
    ALGORITHM=
    
    MAIL_USERNAME=
    MAIL_PASSWORD=
    MAIL_FROM=
    MAIL_PORT=
    MAIL_SERVER=
    
    REDIS_HOST=
    REDIS=