# use 'node' as a base image
FROM node
# setup working directory
WORKDIR /app
# copy file needed for install dependancies
COPY package.json /appdocker
# install dependencies in image
RUN npm install
# copy all files to /app folder in image
COPY . /app
# open 80 port outside of image
EXPOSE 80
# run command 'node server.js' inside container
CMD ["node", "server.js"]