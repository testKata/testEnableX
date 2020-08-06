Before you can run this application by hosting it locally you need to customize server/vcxconfig.js:

Change the file to following :

`voice-api-outbound/config-outbound.js`{{open}}

Add  the following from your config.js


config.app_id = "YOUR_APP_ID";
 // Enter Your App ID that you received from e-mail

config.app_key = "YOUR_APP_KEY";
// Enter Your App Key

Following part of the config is required only if you are running on a server that is unreachable from Voice Server.
This is usually the case of development enviornment 

config.webhook_port = 3000;
config.ngrok = true; // If false, user needs to provide ssl certs


If you have a publicly reachable server, you can add it here as a webhook

In this example the webhook wiuld be:  
config.webhook_host = 'https://[[HOST_SUBDOMAIN]]-80-[[KATACODA_HOST]].environments.katacoda.com'; // Needs to provide if ngrok = false

Since the webhook uses https protocol, you would need to install the certs.




