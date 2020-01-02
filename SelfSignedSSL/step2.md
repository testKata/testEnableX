Generate a CSR (Certificate Signing Request)

Once the private key is generated a Certificate Signing Request can be generated. The CSR is then used in one of two ways. Ideally, the CSR will be sent to a Certificate Authority, such as Thawte or Verisign who will verify the identity of the requestor and issue a signed certificate

 The second option is to self-sign the CSR, which will be demonstrated in the next section.

During the generation of the CSR, you will be prompted for several pieces of information. These are the X.509 attributes of the certificate. One of the prompts will be for "Common Name (e.g., YOUR name)". It is important that this field be filled in with the fully qualified domain name of the server to be protected by SSL. If the website to be protected will be https://public.yourname.com, then enter public.yourname.com at this prompt. The command to generate the CSR is as follows:

Please make sure you use the same password and paraphrase when asked


`openssl req -new -key server.key -out server.csr`{{execute}}

It will display following: 
Country Name (2 letter code) [IN]: IN
// Country name
State or Province Name (full name) [Karnataka]:
Karnataka state // State
Locality Name (eg, city) [Bangalore]:
Bangalore // City
Organization Name (eg, company) [My Company Ltd]:
// Enablexiodemo.com
Organizational Unit Name (eg, section) []:Info
Common Name (eg, your name or your server's hostname) []:
//enablex.io
Email Address []:
//support@vcloudx.com
Please enter the following 'extra' attributes
to be sent with your certificate request
A challenge password []:
An optional company name []:
