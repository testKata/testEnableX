Before you can run this application by hosting it locally you need to customize server/vcxconfig.js:

The sample uses APP_ID and APP_KEY as enviornment variables that you need to export.

Copy and paste your APP_ID from Portal->Project


`export ENABLEX_APP_ID=`{{execute no-newline}}

and hit Enter key <kbd>Enter</kbd>

Copy and paste your APP_KEY from Portal->Project

 
`export ENABLEX_APP_KEY=`{{execute no-newline}}
and hit Enter key <kbd>Enter</kbd>



In this example the webhook would be:  
`export PUBLIC_WEBHOOK_HOST=https://[[HOST_SUBDOMAIN]]-3000-[[KATACODA_HOST]].environments.katacoda.com`{{execute}} // Needs to provide if ngrok = false

Since the webhook uses https protocol, you would need to install the certs.




