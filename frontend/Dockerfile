FROM node:14.15.0
WORKDIR /app
COPY ["package-lock.json", "package.json", "wait-for.sh", "start.sh", "./"]
RUN apt-get update && apt-get install netcat -y && chmod +x ./wait-for.sh ./start.sh && npm install --production
COPY . .
EXPOSE 80
CMD ["npm", "start"]