Before you can run this application by hosting it locally you need to customize server/vcxconfig.js:

vcxconfig.SERViCE = {
  name: "EnableX Sample Web App",     // Name of the Application [Change optional]
  version: "1.0.0",                   // Version [Change optional]
  path: "/v1",                        // Route [Default /v1]
  domain: "yourdomain.com",           // FQDN of  your hosting enviornment
  port  : "443",                     // FQDN of  your hosting port. You need sudo permission if you want to use standard 443
  listen_ssl : true                   // SSL on/off key  [ Set always to "true" ]
};

vcxconfig.Certificate = {
  ssl_key:    "../certs/yourdomain.key",  // Use the certificate ".key" [self signed or registered]
  ssl_cert :  "../certs/yourdomain.crt",  // Use the certificate ".crt" [self signed or registered]
  sslCaCerts :  ["../cert/yourdomain.ca-bundle"]    // Use the certificate CA[chain] [self signed or registered]
};

vcxconfig.SERVER_API_SERVER = {
  host: 'api.enablex.io',             // Hosted EnableX Server API Domain Name
};

vcxconfig.clientPath  = "../client";    // UI files location
vcxconfig.APP_ID      = "YOUR_APP_ID";  // Enter Your App ID
vcxconfig.APP_KEY     = "YOUR_APP_KEY"; // Enter Your App Key
