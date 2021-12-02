FROM node:14
WORKDIR /usr/src/app
COPY /example-frontend /usr/src/app
RUN npm install

RUN npm run build

RUN npm i -g serve

CMD ["serve", "-s", "-l", "5000", "build"]

#CMD LINE: docker build . -t front && docker run -p 5000:5000 front