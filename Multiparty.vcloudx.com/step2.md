Before you can run this application by hosting it locally you need to customize server/vcxconfig.js:

Change the file to following :

`Multiparty-Audio-Chat-Open-Source-NodeJS-Application/server/vcxconfig.js`{{open}}

change the following from your config.js

port  : "4443",  // FQDN of  your hosting port

vcxconfig.APP_ID      = "YOUR_APP_ID"; 
 // Enter Your App ID that you received from e-mail

vcxconfig.APP_KEY     = "YOUR_APP_KEY"; 
// Enter Your App Key


Run npm install --save to build the project and the build artifacts will be stored in the ./node_modules directory.

`npm install --save`{{execute}}

Now lets install the Self-Signed Certificates.

Make a directory called certs

`mkdir certs `{{execute}}

Change to certs directory

`cd certs `{{execute}}

Create and Install certificates 

`openssl req -nodes -new -x509   -keyout katakoda.key -out katakoda.crt   -days 365   -subj '/CN=katakoda.com/O=My Company Name LTD./C=US'; cat katakoda.crt > katakoda.ca-bundle `{{execute}} 


Install node 

`npm install --save`{{execute}}

Run node server.js inside server folder for starting your Server.

Change to server

`cd  server`{{execute}}

`node server.js`{{execute}}
