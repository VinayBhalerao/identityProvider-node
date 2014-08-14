## 3scale Identity provider with Oauth 2.0 authorization code flow with nginx

This tutorial is a sample IDP developed by 3scale to give you a look and feel how an Identity provider connects and exchanges messages between

1. Google Playground - Client Application
2. Identity provider - Developed in node.js and mongoDB as database to store the user credentials
3. Nginx - Authorization endpoints 
4. Redis server - To store the access_tokens
5. 3scale - Authorization backend for validating the tokens and generating the client_id and client_secret

##Prerequisites
1. Install node with version v0.10.29 or higher
2. Install MongoDB on localhost or use the [Modulis.io](https://modulus.io/)to create MongoDB setup online. After installation, edit the config/database.js with the mongoDB url
`mongodb://<user>:<pass>@mongo.onmodulus.net:27017/Mikha4ot`, if Modulus.io is used to create DB OR `mongodb://127.0.0.1/mydb`, if localhost is used to create setup

##Steps
1. Clone the repo: `git clone git@github.com:VinayBhalerao/identityProvider-node.git`
2. Install the packages `npm install`
3. Change the config/database.js with the url given in prequisites section
4. Start the server: `node server.js`

