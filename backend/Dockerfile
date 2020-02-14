#import image from node / alpine is a tiny image
FROM node:12.4.0-alpine

#create a node module folders and set the permission of the folder
RUN mkdir -p /home/node/api/node_modules/ && chown -R node:node /home/node/api

#setting the work directory folder
WORKDIR /home/node/api

#copy folder contet to /home/node/api on container // remember to set the permission as node user
COPY --chown=node:node . /home/node/api

#force to use node user
USER node

#install all dependencies
RUN npm install -qy

#expose the 3333 port
EXPOSE 3333

#run the node server
CMD ["npm", "start"]
