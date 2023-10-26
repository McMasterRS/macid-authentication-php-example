# php-sso-example
A sample project that shows developers how they can add Single Sign-On (SSO) to their PHP web application to allow users to sign using their MacID credentials.

## Build

### Requirements

- [Docker](https://docs.docker.com/engine/install/) 20.10 or newer
- [docker-compose](https://docs.docker.com/compose/install/) 1.29 or newer

### Usage

Before building the container, open the `data/index.php` file and fill out the the following values:
- `client_id` in `$requestData`
- `client_secret` in `$requestData`
- `{tenant}` in all strings where it appears
- `{client_ind}` in all strings where it appears

To build and run the container, simply run:  
```bash
docker-compose -p $USERNAME-container up --build
```
