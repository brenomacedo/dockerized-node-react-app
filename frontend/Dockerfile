FROM node:14.15.0
WORKDIR /app
COPY ["package-lock.json", "package.json", "./"]
RUN npm install --production
COPY . .
EXPOSE 80
CMD ["npm", "start"]