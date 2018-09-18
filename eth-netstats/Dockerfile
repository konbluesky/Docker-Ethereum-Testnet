FROM node:8

RUN apk add --update git

RUN git clone https://github.com/cubedro/eth-netstats

WORKDIR /eth-netstats

RUN npm install --registry=https://registry.npm.taobao.org
RUN npm install -g grunt-cli --registry=https://registry.npm.taobao.org
RUN grunt

EXPOSE 3000

CMD ["npm", "start"]
