#everything runs on node so lets start with that as a base (this gets a base node image from docker's online registry - like their version of github/bitbucket but for vm images)
FROM node

#we need webpack
RUN npm install webpack -g

#and yarn is the dependencie manager of choice these days!


#Now to set up our playground (this is like "cd"ing into /fed)
WORKDIR /fed

#now let's get the src code into the container (I imagine this as creating a kind of tunnel (worm hole?) between the host OS and the docker container)
VOLUME ./src /fed/src