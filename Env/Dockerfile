FROM node:18
WORKDIR /Demo-React
COPY . .
#RUN npm cache clean --force
#RUN rm -rf node_modules
#RUN rm -f package-lock.json
#RUN mkdir log
#RUN ls -l
RUN npm install
RUN npm run build
RUN npm install -g serve@13.0.4 
CMD [ "serve", "-s", "-l", "3000", "build" ]
#WORKDIR dist
#ENV AWS_ACCESS_KEY_ID=""
#ENV AWS_SECRET_ACCESS_KEY=""
#ENV KMS_DATA_KEY=''
#ENV AWS_REGION='us-east-1'







