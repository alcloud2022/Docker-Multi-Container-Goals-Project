#Node version
FROM node 

#Working directory set to app
WORKDIR /app

#Copy package into the working directory
COPY package.json .

#intsall the necessary packages/dependancies
RUN npm install

#copy all remaining code to the working directory
COPY  . .

#Expose port 80
EXPOSE 80

ENV MONGODB_USERNAME=root
ENV MONGODB_PASSWORD=secret

#Run the application
CMD ["npm", "start"]