# Base image
FROM node:alpine

# Specify base workdir inside the container
WORKDIR /user/app

#Copy package to avoid invalidation of a cache.
COPY ./package.json ./

# Install deps 
RUN npm install

# Copy everything else
COPY ./ ./

# Default command

CMD ["npm", "start"]
