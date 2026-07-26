FROM node:alpine

#Create a new user and group called 'app' and add the user to the group
#-S flag creates a system user, which is a user that is not intended to log in to the system. This is a good practice for running applications in containers, as it reduces the risk of privilege escalation attacks.
#-G flag specifies the group that the user should be added to. In this case, we are adding the 'app' user to the 'app' group.
RUN addgroup -g 1001 app && adduser -D -u 1001 -G app app

USER app    

WORKDIR /app

COPY package*.json ./

USER root

RUN chown -R app:app . 

RUN npm install

COPY . .

EXPOSE 3000

CMD ["npm", "run", "dev"]

