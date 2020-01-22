# Wordpress With Docker

As we know that WordPress is one of the most popular content management system (CMS). Running WordPress typically involves Apache, MySQL and PHP which is time-consuming. This is where Docker comes in to simplify the installation process. Installing WordPress with Docker is a breeze.
Let's see how you can setup Wordpress with docker?? 

## Why should we use docker??
Many of you are thinking that why should we use docker. so the answer is using docker you don't need xampp or any other big stack tools to be installed. All of you needs to know is how to run docker containers. You only needs to create one simple file with .yml or .yaml extension to setting up the wordpress.

## What is yaml
yaml is basically a human-readable structured data format. It is same as XML or JSON file but It is less complex than XML or JSON. It essentially allows you to provide all the powerful configuration settings like MYSQL, phpmyadmin etc.

Let see step by step how to setup wordpress with docker.

## Install Docker
First of all you have to install docker in your system. you can check documentation on https://docs.docker.com/ for installing docker in varios systems like windows, ubuntu, debian, mac etc.

## Create .yml or .yaml File
After successfully installing docker. Now, create docker-compose.yml or docker-compose.yaml. I have created docker-compose.yaml.
Now, add all the required services you want to include inside your docker-compose.yaml file like db which is for creating nd mananing database, wordpress for setting up wordpress, phpmyadmin for accessing and managing your phpmyadmin etc. 

## Run Your Compose File
After adding all the details inside your docker-compose.yaml file open your terminal and run following command.
```
docker-compose up -d
```
It will create network with the name of your folder name, Volume , Database etc. After running above command you can see all the required folders and files of wordpress are added inside your folder.

## Install Wordpress
open your browser and type http://localhost:8000. It will be taken you to wordpress installation page. Enter all the details like sitename, username, password, email etc. and click on install. Thats' it you have successfully installed wordpress using docker.

If you want to access your phpmyadmin then simple type  http://localhost:8080 and it enter your phpmyadmin username and password you have setted inside your docker-compose file. You can see your all the databases there.

Thank You Guys!!!!
