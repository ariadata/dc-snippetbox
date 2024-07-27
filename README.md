# snippet-box with with docker-compose
[![Build Status](https://raw.githubusercontent.com/ariadata/ariadata-files/main/public-assets/images/ariadata_logo.png)](https://ariadata.co)

![](https://img.shields.io/github/stars/ariadata/dc-snippetbox.svg)
![](https://img.shields.io/github/watchers/ariadata/dc-snippetbox.svg)
![](https://img.shields.io/github/forks/ariadata/dc-snippetbox.svg)

### This needs : [dockerhost](https://github.com/ariadata/dockerhost-sh) + [nginx-proxy-manager](https://github.com/ariadata/dc-nginxproxymanager)

---
#### 1- Clone this repo and pull the image :
```sh
git clone https://github.com/ariadata/dc-snippetbox.git
cd dc-snippetbox
rm -rf .git
docker-compose pull
```
---
#### 2- Edit `.env` and `docker-compose.yml` as you need.

#### 3- Run docker-compose file by using :
```sh
docker-compose up -d
```
#### 4- Goto Nginx-Proxy-Manager admin panel and add this stack as proxy-host :
> Domain : `Your-FQDN` you must pointed it before!
> 
> Schema : `http`
> 
> Name or IP : `snippetbox`
> 
> Port : `5000`
>
> Config SSL Part

#### 5- goto : `https://Your-FQDN/`

Done!


