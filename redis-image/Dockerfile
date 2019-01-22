#Use an existing Docker iumage as a base
FROM alpine

#Download and install a dependency
RUN apk add --update gcc
RUN apk add --update redis

#Tell the image what to do when it starts as a containter
CMD ["redis-server"]
