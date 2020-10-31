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

Set Up WordPress:-

 1.Create a new directory in your home folder called my_wordpress and cd into it:

    mkdir ~/my_wordpress/
    cd ~/my_wordpress/
 2.Create a file named docker-compose.yml in this folder and add the following contents. Set your own passwords for the WORDPRESS_DB_PASSWORD, MYSQL_ROOT_PASSWORD, and MYSQL_PASSWORD environment options. The password entered for WORDPRESS_DB_PASSWORD and MYSQL_PASSWORD should be the same.
 
 3. From the my_wordpress directory, start your Docker containers:

      docker-compose up -d    
 
 4.The Docker containers will take a minute or two to start up WordPress and MySQL. Afterwards, you can visit your Linode’s IP address in your web browser and you should be directed to the WordPress setup form.

