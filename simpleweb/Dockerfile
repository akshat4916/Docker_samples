# Specify base image
FROM node:alpine

#Install some dependencies
WORKDIR /usr/app
COPY ./package.json ./
RUN npm install

# don't run npm install after any change in main code
COPY ./ ./

#DEFAULT command
CMD ["npm","start"]

#2 ways to have npm installed - 
# use image which has node already installed
# or install node manually using RUN commands