At this point we have following things ready:

1. Phone number configured for the outbound dialing 
2. changes done to the configurations

Now install the nodejs and start the application.

Run npm install --save to build the project and the build artifacts will be stored in the ./node_modules directory.
`npm install --save`{{execute}}

Run node server.js inside server folder for starting your Server.


`node client-outbound.js`{{execute}}

Now you can open browser at :

https://[[HOST_SUBDOMAIN]]-80-[[KATACODA_HOST]].environments.katacoda.com

"environment": {
    "showdashboard": true,
    "dashboards": [{"name": "URL", "href": "https://www.katacoda.com"},
        {"name": "Port :80", "port": 80},
        {"name": "Placeholder", "href": "https://[[HOST_SUBDOMAIN]]-80-[[KATACODA_HOST]].environments.katacoda.com"}],
    "uilayout": "terminal-iframe"
}
