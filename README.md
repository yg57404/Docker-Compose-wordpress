# Docker-wordpress
Install WordPress with Docker Compose

Install Docker Compose

1. Run this command to download the current stable release of Docker Compose:

    sudo curl -L "https://github.com/docker/compose/releases/download/1.27.4/docker-compose-$(uname -s)-$(uname -m)" -o /usr/local/bin/docker-compose

2. Apply executable permissions to the binary:

    sudo chmod +x /usr/local/bin/docker-compose

Note: If the command docker-compose fails after installation, check your path. You can also create a symbolic link to /usr/bin or any other directory in your path.

For example:

sudo ln -s /usr/local/bin/docker-compose /usr/bin/docker-compose

   1.Optionally, install command completion for the bash and zsh shell.

   2.Test the installation.

$ docker-compose --version
docker-compose version 1.27.4, build 1110ad01
