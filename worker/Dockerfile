FROM node:11.10.1-alpine

WORKDIR /app
COPY ./package.json .
RUN npm install
RUN npm audit fix
COPY . .
CMD ["npm", "run", "start"]