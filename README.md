# php-sso-example

A sample project that shows developers how they can add Single Sign-On (SSO) to their PHP web application to allow users to sign using their MacID credentials.

## Build

### Requirements

- [Docker](https://docs.docker.com/engine/install/) 20.10 or newer
- [docker-compose](https://docs.docker.com/compose/install/) 1.29 or newer

### Usage

Before building the container, duplicate the `config/.env.sample` file to a new file named `config/.env`. Fill out all the information required in the `config/.env` file.  

To build and run the container, simply run:  
```bash
docker-compose -p $USERNAME-container --env-file config/.env --file docker-compose.yaml up --build
```
