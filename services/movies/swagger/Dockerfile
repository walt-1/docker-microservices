FROM node:latest

# set working directory
RUN mkdir usr/src/app
WORKDIR usr/src/app

# add path
ENV PATH /usr/src/node_modules/.bin:$PATH

#install and cache dependencies
ADD package.json /usr/src/app/package.json
RUN npm install

CMD ["npm", "start"]
