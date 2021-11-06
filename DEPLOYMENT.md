# SeaLit Catalogues Deployment

## Prerequisites and the requirements

1. The latest version of NodeJs.
2. Angular CLI  
  After downloading nodeJs run `npm install -g @angular/cli`
3. Java
4. Tomcat

## Installing node modules

1. Go to \seaLit and run => `npm install`
2. Go to \api and run => `npm install`

## Change the Ip of the API

- In the angular project go to seaLit\src\app\services\list.service.ts and in line 11 change the Ip to the Ip of the computer that th api.js will run on.

## Production build for Angular Application

- Go to /seaLit and run => `ng build --base-href=/seaLit/`
This will compile an Angular app into an output directory named dist/seaLit

## Run API

- Go to /api and run => `npm run server`

## deployment to tomcat server

1. In the abgular application go to seaLit/dist and copy the folder seaLit
2. Then go to your tomcat server etc. Tomcat 10.0\webapps and paste thr folder
3. After that go to Tomcat 10.0\bin and click on Tomcat10.exe
4. Open a browser to <http://localhost:8080/seaLit/>