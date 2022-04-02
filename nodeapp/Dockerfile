FROM node:lts-alpine
ENV NODE_ENV=production
WORKDIR /usr/src/catbot-9000
COPY ["package.json", "package-lock.json*", "npm-shrinkwrap.json*", "./"]
RUN npm install && mv node_modules ../
COPY . .
EXPOSE 3000
CMD ["npm", "run dev"]
