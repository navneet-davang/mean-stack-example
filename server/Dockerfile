FROM node:latest
WORKDIR /server/app
COPY . /server/app/
RUN npm install
RUN npm run build
EXPOSE 5200
CMD ["node", "dist/server.js"]
