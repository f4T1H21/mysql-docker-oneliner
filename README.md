# MySQL Docker One-Liner
This bash script first pulls `mysql:latest` docker image if you don't have. Once you have the mysql docker image, it runs two different containers simultaneously where one of them is a MySQL server and the other is an interactive MySQL client which connects back to the server. After you `exit` MySQL, the client container will be killed and removed as well as the server container. Therefore __do not try to develop projects on both containers because they won't exist after you exit!__

## Use Side
If you are working on database behaviours or learning MySQL and want containers and processes to be cleaned up automatically after the work, this one-liner script is definitely for you!

## Dependencies:
- [`sudo`](https://www.sudo.ws/getting/packages/)
- [`docker`](https://docs.docker.com/get-docker/)
- [`jq`](https://stedolan.github.io/jq/download/)

## Getting started:
```bash
$ git clone https://github.com/f4T1H21/mysql-docker-oneliner
$ cd mysql-docker-oneliner
$ chmod +x mysql-oneliner.sh
$ ./mysql-oneliner.sh
```

## PoC:
![PoC](poc.gif)

<br>

___─ Written by Şefik Efe ─___