# Post to Generic Streaming Channel Demo

Basic node.js app to post to a Salesforce generic streaming channel using Express, nForce, and Jade templating library.

This works with the Generic Streaming API [demo component](https://github.com/developerforce/SalesforceDurableGenericDemo) you can install in your Salesforce org.

For more information on the Streaming API, generic streaming events, and the new durable streaming features I recommend reading the [doc](https://developer.salesforce.com/docs/atlas.en-us.api_streaming.meta/api_streaming/) on Salesforce Streaming API and watching the Dreamforce 15 [video](http://salesforce.vidyard.com/watch/AR1zoCe8LIVTAcr29qIGmA) given by the product team leads Product Manager [Jay Hurst](https://twitter.com/extraidea) and lead developer [John Brock](https://twitter.com/_johnbrock).

Horribly hacked into place from Jeff Douglas' nForce demo app.

## Deploy to Heroku

Deploy this app to Heroku for free and have it up and running in a matter of minutes.

[![Deploy](https://www.herokucdn.com/deploy/button.png)](https://heroku.com/deploy?template=https://github.com/pchittum/durable-stream-post-message)

## Local Installation Instructions

From the command line type in:

```
git clone git@github.com:pchittum/durable-stream-post-message
cd durable-stream-post-message
npm install
```

### Node Module Dependencies

These will be automatically installed when you use any of the above *npm* installation methods above.

1. [express](http://expressjs.com/) - framework
2. [nforce](https://github.com/kevinohara80/nforce) - REST wrapper for force.com
3. [async](https://github.com/caolan/async/) - asynchronous utility module
4. [jade](http://jade-lang.com/) - the view engine

### Running the Application Locally

1. Open terminal and change directory to node-nforce-demo root
2. `node app.js`
3. Point your browser to: [http://localhost:3001](http://localhost:3001)

### Deploying to Heroku

```
heroku create
heroku config:add CLIENT_ID=YOUR-SALESFORCE-CLIENT-ID
heroku config:add CLIENT_SECRET=YOUR-SALESFORCE-SECRET
heroku config:add USERNAME=YOUR-SALESFORCE-USERNAME
heroku config:add PASSWORD=YOUR-SALESFORCE-PASSWORD-AND-TOKEN
heroku open
```

### Demo on Heroku

This application is running on heroku at: [http://durable-stream.herokuapp.com/](http://durable-stream.herokuapp.com/)

## Contributors
* Peter Chittum -> [pchittum](https://github.com/pchittum)

## Credits
* Jeff Douglas (original project) -> [jeffdonthemic](https://github.com/jeffdonthemic)
