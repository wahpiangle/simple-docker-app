#parent image
FROM node:18.15.0-alpine

# this command specifies that the commands will be done from this directory
WORKDIR /app

# . indicates the current directory
# this command will copy all the files from the current directory to the /app directory in the container
COPY . .

RUN npm install

EXPOSE 4000

# use of CMD as opposed to RUN is that CMD is executed when the container is run not when it is being built
CMD [ "node", "app.js" ]