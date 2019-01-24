FROM node:alpine as builder
WORKDIR '/app'
COPY package.json .
RUN npm install
COPY . .
RUN npm run build

FROM nginx
COPY --from=builder /app/build /usr/share/nginx/html
#default command for this is to start nginx - do not need to specify anything elsre
# docker run d2dc6bfae5a0 -p 8080:80
