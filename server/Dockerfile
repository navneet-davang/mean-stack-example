# Use the official lightweight Node.js 12 image.
# https://hub.docker.com/_/node
FROM node:18-slim

WORKDIR /usr/app
COPY ./ /usr/app
COPY .env* /usr/app

# Install dependencies and build the project.
RUN npm install
RUN npm run build

EXPOSE 5200
# Run the web service on container startup.
CMD ["node", "dist/server.js"]