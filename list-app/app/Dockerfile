FROM node:12-alpine
# we're saying to start from image called 'node:12-alpine'. It's not on my system, so docker downloads it
RUN apk add --no-cache python g++ make
WORKDIR /app
# set the working directory of the image(?)
COPY . .
RUN yarn install --production
# use yarn to install dependencies
CMD ["node", "src/index.js"]
# CMD specifies to run default command when container started from this image