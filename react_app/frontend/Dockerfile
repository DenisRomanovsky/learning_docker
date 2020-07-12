# Dependencies and build
# ======================
FROM node:alpine as builder
WORKDIR '/app'
COPY package.json .
RUN npm install
COPY . .
CMD ["npm", "run", "build"]

# Ngnix and prod
# ======================
FROM nginx
COPY --from=builder /app/build  /usr/share/nginx/html
# nginx will start automatically
