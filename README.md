#usage  2020



 vi .env
DATA_PATH_HOST 改成你要的目录
 例如 /data/www


然后   prod-sns-pc 改成你的项目名 docker-compose.yml
- ${DATA_PATH_HOST}/prod-xx-pc:/data/app

也就你的 宿主机 目录为
ls /data/www/prod-xx-pc

 docker-compose up -d nuxt-pc

# docker-compose-nuxt

node.js docker容器化挂载

```bash
cp .env.example .env
```

按照自己的需要更改.env配置文件，当前主要是用了${DATA_PATH_HOST} 这个变量，为挂载目录,根据自己的需求自行更改！

```bash
docker-compose up -d nuxt 
docker-compose up -d nuxt-mobile
```

