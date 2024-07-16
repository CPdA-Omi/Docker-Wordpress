# Docker Wordpress

Temporary repository for the Wild Code School.

## Prerequisites

**You need to have [docker](https://docs.docker.com/engine/install/) installed in your computer**

### Environments variables

Then, your files should resembles to this:

```bash
├── compose.yml
├── .env
├── .git
│   └[...]
└── .secrets
    ├── db_name.txt
    ├── db_root_password.txt
    ├── db_username.txt
    └── db_user_password.txt
```

Add those 4 files in the `.secrets` directory and enter values inside:

- `db_name.txt` is for your database name,
- `db_root_password.txt` is for the password of your root password of the database,
- `db_username.txt` is the user you should use while runing Wordpress,
- `db_user_password.txt` is the password of the user of the database (should be used while runing Wordpress.

## Launching

To launch it, you need to be in the cloned directory and then enter `docker compose up` command (plus `-d` option if you want to launch it in the background).

If you correctly added the files in the `.secrets` directory, all should be in place correctly.

## Other actions

- `docker compose stop` to stop the containers,
- `docker compose start` to start containers when they are stopped,
- `docker compose down` to delete the containers from your computer (with the `-v` option if you want to delete the saving volumes too).
