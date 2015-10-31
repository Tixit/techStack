# techStack
A recommended technology stack of open-source modules.

I believe frameworks are inherently bad design. Frameworks are bloated. Frameworks are opinionated. Frameworks lock you in. 

Instead, I believe the best design approach is to build a system with lots of independant components that work together in harmony, but where any one can be swapped out as needed. This is the list of recommended libraries to build a robust dynamic web application, almost all of which we currently use at Tixit:

## Backend

* [node.js](http://nodejs.org/) - What better way to create synergy between your frontend and backend than by using the same language? Also good at handling thousands of websocket connections per machine.
* [webpack](http://webpack.github.io/) - An excellent CommonJS script bundle creator. It creates efficient production bundles that can be lazy loaded, and makes development incredibly easy with its 'watcher' functionality that rebuilds your package automatically on-change of source files.
* [MongoDB](http://www.mongodb.org/) - One of the most popular no-sql database systems.
* [fibers/futures](https://github.com/laverdet/node-fibers) - The futures here make all your async look like its synchronous. Its fantastic!
* [websockets](https://github.com/theturtle32/WebSocket-Node) - There may be better websocket libraries out there, but this is the one we're currently using. 
* [colors](https://github.com/marak/colors.js/) - Make your console output colorful, so it doesn't hurt your eyes!
* [incremental-installer](https://github.com/fresheneesz/incremental-installer) - Do you have initialization scripts that need to be run once and only once on each machine? This modules helps your team do that in a distributed way!
* [scrypt](https://github.com/barrysteyn/node-scrypt) - Modern secure password handling made easy. 

## Frontend

* [Gem.js](https://github.com/Tixit/Gem.js) - A view library for build modular, composable web components and styles in pure javascript.
* [websockets](https://developer.mozilla.org/en-US/docs/WebSockets) - Need to send the browser more data right now? Also, websockets can be use [beyond the browser](http://www.slideshare.net/cjmyers/web-sockets-are-not-just-for-web-browsers-26442068)
* [bluebird promises](https://github.com/petkaantonov/bluebird) - Meticulously optimized future/promise library, that allows working asynchronously with familiar try-catch semantics. Bluebird also has a non-bloated set of powerful utilities, also meticulously optimized.
* [observe](https://github.com/Tixit/observe) - React when your data objects change.
* [grapetree](https://github.com/fresheneesz/grapetree) - A simple hierarchical path routing system. 
* [modernizr](http://modernizr.com/) - A feature detection library that allows you to detect feature deficits and fix them with polyfills.

## Both

* [proto](https://github.com/fresheneesz/proto) - A class/prototype creation library.
* [deadunit](https://github.com/fresheneesz/deadunit) - A simple unit testing system that focuses on making test driven development as easy as possible.
* [syn](https://github.com/bitovi/syn) - Generate synthetic events that look just like user generated mouse clicks and key presses!
* [moment](http://momentjs.com/) - Time handling done right.

## Development

* [Vagrant](https://www.vagrantup.com/) - Very useful for developing in a linux environment when you're running windows.

## Things we haven't open sourced

* wsRpc - We've built an RPC protocol on top of websockets that we'll probably open source at some point.
* 
