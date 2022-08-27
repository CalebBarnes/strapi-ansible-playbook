# strapi-ansible-playbook

A [WIP] blueprint to automate the deployment of strapi servers.

### What it does
- setup passwordless sudo
- creates sudo user
- copy ssh key
- disable root password auth
- apt install `curl`, `vim`, `git`, `ufw`, `build-essentials`, `nginx`, `certbot`, & `python3-certbot-nginx`
- install `nvm`
- install `node` with `nvm`
- install `yarn`
- install `pm2`

- create nginx config with reverse proxy and https
- symlink new nginx config into `sites-enabled`
- initialize certbot for nginx
- schedule cron to renew certbot Let's Encrypt certificates

- configure firewall to block everything except for ssh and nginx


todo:
- install postgres
- create postgres user
- create postgres db
- clone strapi project github repo from variable
- set strapi envs to connect it to the postgres db
