#import image from node on docker hub
FROM node:12.4.0-alpine

#create directory node modules and set permission as node
RUN mkdir -p /home/node/frontend/node_modules/ && chown -R node:node /home/node/frontend

#setting the work directory folder
WORKDIR /home/node/frontend

#copy the content to the directory
COPY --chown=node:node . /home/node/frontend

#set user as node
USER node

#run and install node dependencies
RUN npm install -qy

#expose port 3000
EXPOSE 3000

#run npm start command
CMD ["npm", "start"] 