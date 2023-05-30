FROM node
WORKDIR /var/www/myapp
COPY package.json ./
RUN npm install
COPY . .
COPY .env.docker ./.env
EXPOSE 4300 4301
RUN npm run build
CMD ["npm", "run", "run:prod"]