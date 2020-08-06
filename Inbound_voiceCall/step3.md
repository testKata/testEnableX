In case you are choosing to run over ngrok you can skip this scenario.
But if you choose to continue without ngrok please follow these steps 

Now lets install the Self-Signed Certificates.

Make a directory called certs

`mkdir certs `{{execute}}

Change to certs directory

`cd certs `{{execute}}

Create and Install certificates

`openssl req -nodes -new -x509   -keyout example.key -out example.crt   -days 365   -subj '/CN=katakoda.com/O=My Company Name LTD./C=US'; cat example.crt > example.ca-bundle`{{execute}}

Change back to the main dir


`cd ..`{{execute}}


