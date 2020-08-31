# Ghost CMS + Docker Compose

These are some reassons why use this Docker Compose in your production environment.

☝️ 2 command to install

👨‍💻 Ready to production and local development

⚡ Performance Optimized

🔒 SSL auto-renewed

## Stack

- Ubuntu 20.04 LTS or Centos 8
- Ghost CMS lastest docker image(alpine)
- MariaDB latest docker image
- Nginx latest docker image(alpine)
- Letsencrypt latest docker image
- Docker
- Docker-compose

## How start using this source?

Then copy this command below and **change the mydomain.com to your domain** and **change the email@email.com to your email address** and run it inside your new server. Make sure that your domain is pointing to your server IP.

### For Ubuntu 20.04 LTS users

```bash
sudo apt update -y && sudo apt upgrade -y && sudo apt install curl git -y && sudo apt autoremove -y
```

```bash
curl -s https://raw.githubusercontent.com/woosungchoi/ghost-cms/master/dc | bash -s setup mydomain.com email@email.com
```

### For Centos 8 users

```bash
sudo yum -y update && sudo yum install -y curl git
```

```bash
curl -s dcc https://raw.githubusercontent.com/woosungchoi/ghost-cms/master/dcc | bash -s setup mydomain.com email@email.com
```

## How start using locally?

In your local environment you need to have installed:

- Docker
- Docker Compose

After clone this repository, you can access the `dev` folder to be able to run the local dev environment using this command below.

```bash
git clone https://github.com/woosungchoi/ghost-cms.git ghost
cd ghost/dev
docker-compose up -d
```

🎉Done! Access your https://localhost/ghost to access the admin panel and create your account.

## Commands

| Commands  | Description  |
|---|---|
| `./dc start`  | Start your containers  |
| `./dc stop`  | Stop all containers  |
| `./dc update`  | Get Ghost updates and restart containers |

Thank you all [contributor](https://github.com/clean-docker/ghost-cms/graphs/contributors)!
