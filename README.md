# code-duck
code-server in docker
## Prerequisite
* docker installed
* git installed
## Steps
1. Clone this repo
```console
git clone https://github.com/frakw/code-duck.git
```
2. Copy new one
```console
cp -r code-duck myname
cd myname
```
3. Config `docker-compose.yaml` \
![](./imgs/1.png)
* Change myname into the name you want
* Change the expose port 8880 into the port you want
4. Config `root/.config/code-server/config.yaml` \
![](./imgs/2.png)
* Change password into the password you want
5. Deploy docker container
```console
docker compose up -d
```
6. Access <<your-ip:port>> through browser \
![](./imgs/3.png)
* Enter the password you type before
7. Start editing you code
![](./imgs/4.png)
8. Run command in terminal
![](./imgs/5.png)
7. (optional) Add into cloudflare tunnel  \
![](./imgs/6.png)
* You should build up your cloudflare tunnel first
* Type the subdomain you want
* Select `HTTP` then enter local ip and port 