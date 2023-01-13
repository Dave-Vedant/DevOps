# BluePrint of our docker image

FROM node:13-alpine

ENV MONGO_DB_USERNAME = admin \
    MONGO_DB_PWD = password

# create the con964f270f496dtinaer direcoty /home/app
RUN mkdir -p /home/app  

# copy everything to container directory (home/app)
COPY ./app /home/app

# set working directory
WORKDIR /home/app

# will execute  the npm install to install the rquried packages to dir
RUN npm install

# use the  container directory beside of /home/app
CMD ["node", "server.js"]

