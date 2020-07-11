# Base image
FROM node:alpine

#Copy setup to docker image
COPY ./ ./

# Install deps 
RUN npm install

# Default command

CMD ["npm", "start"]
