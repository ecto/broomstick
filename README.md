#broomstick

Lightweight streaming and in-memory caching static file middleware for Director

![broomstick](http://i.imgur.com/B2UpG.jpg)

##install

    npm install broomstick

##usage

````javascript
var director = require('director'),
    broomstick = require('broomstick'),
    router = new director.http.Router();

var static = new broomstick({ path: 'public' });

router.get('*', static);
router.get('/', static);

var server = http.createServer(router.dispatch);

server.listen(8080);
````
