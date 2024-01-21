#install node16 LTS
FROM node:16-alpine

#default port
EXPOSE 5000

WORKDIR /usr/src/app

COPY . .

#install npm packages and generate build
RUN npm install
RUN npm run build

#install serve npm package
RUN npm install -g serve

#command to start app
CMD ["serve", "-s", "-l", "5000", "build"]