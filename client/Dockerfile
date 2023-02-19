FROM node:18-slim AS build

WORKDIR /usr/src/app
COPY package.json package-lock.json ./

# Install dependencies and copy them to the container
RUN npm install
COPY . .

EXPOSE 4200
# Run the web service on container startup.
CMD ["npm", "start"]