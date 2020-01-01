Generate a Private Key

Please make sure you have installed openssl on your server to generate the key

The openssl toolkit is used to generate an RSA Private Key and CSR (Certificate Signing Request). It can also be used to generate self-signed certificates which can be used for testing purposes or internal usage.

The first step is to create your RSA Private Key. This key is a 1024 bit RSA key which is encrypted using Triple-DES and stored in a PEM format so that it is readable as ASCII text.


`openssl genrsa -des3 -out server.key 1024`{{execute}}

Above coomand will ask you for the password and parapharse.
Please enter and note it down to the safe place 
as it will be required for the next step

