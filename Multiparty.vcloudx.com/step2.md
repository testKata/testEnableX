Before you can run this application by hosting it locally you need to customize server/vcxconfig.js:

Change the file to following :

`Multiparty-Audio-Chat-Open-Source-NodeJS-Application/server/vcxconfig.js`{{open}}

Add  the following from your config.js


vcxconfig.APP_ID      = "YOUR_APP_ID"; 
 // Enter Your App ID that you received from e-mail

vcxconfig.APP_KEY     = "YOUR_APP_KEY"; 
// Enter Your App Key



Now lets install the Self-Signed Certificates.

Make a directory called certs

`mkdir certs `{{execute}}

Change to certs directory

`cd certs `{{execute}}

Create and Install certificates 

`openssl req -nodes -new -x509   -keyout example.key -out example.crt   -days 365   -subj '/CN=example.com/O=My Company Name LTD./C=US'; cat example.crt > example.ca-bundle`{{execute}} 

Change back to the main dir


`cd ..`{{execute}}

Install node 

Run npm install --save to build the project and the build artifacts will be stored in the ./node_modules directory.
`npm install --save`{{execute}}

Run node server.js inside server folder for starting your Server.


`node server.js`{{execute}}


https://[[HOST_SUBDOMAIN]]-80-[[KATACODA_HOST]].environments.katacoda.com
