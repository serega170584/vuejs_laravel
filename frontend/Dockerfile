FROM alpine:3.18

WORKDIR "/app"

RUN apk add --update nodejs npm
RUN npm install --global yarn
RUN yarn global add @vue/cli
RUN yarn install

RUN addgroup -g 1000 app && adduser -u 1000 -G app -s /bin/sh -D app

CMD yarn serve