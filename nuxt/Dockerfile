FROM node:12.18.2-alpine3.12

MAINTAINER linuxsa.org
RUN sed -i 's/dl-cdn.alpinelinux.org/mirrors.aliyun.com/' /etc/apk/repositories 

RUN apk --update add wget \
  curl \
  git \
  build-base 

RUN apk add busybox-extras

#RUN   apk add --update --no-cache gmp gmp-dev 
#RUN   apk add --update --no-cache gmp gmp-dev 
#RUN     docker-php-ext-install gmp 



WORKDIR /data/app

EXPOSE 3333 
#EXPOSE 3333 3334
#CMD ["yarn", "postinstall"]
ENTRYPOINT ["yarn","start"]

