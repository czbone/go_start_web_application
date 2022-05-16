FROM golang:alpine

RUN apk update
RUN apk add git

# for building optional Analysis Tools
RUN apk add build-base

# set timezone
RUN apk add --update --no-cache tzdata \
  && cp /usr/share/zoneinfo/Asia/Tokyo /etc/localtime \
  && echo "Asia/Tokyo" > /etc/timezone \
  && apk del tzdata
