Chatterbox server
==============

This is a project I completed with a pair as a student at Hack Reactor. It is a server application which contains utilities with routing and works with the [Chatterbox client](https://github.com/dhuang919/Chatterbox-client) as a replacement for the Parse API back-end.

## Structure:

The repository consist of

- Server app
- [Client app](https://github.com/dhuang919/Chatterbox-client)
- Spec files

#### Chatterbox server

The server features at a glance:

- GET/POST/OPTIONS requests
- Support CORS to handle cross domain issues
- Serve Static Assets (CSS/HTML/JS/img)
- Persistent storage on file

Its architecture allows the app to easily extend the request handler router and add as many endpoints as needed.

## Install:

The app relies on bower and npm for managing external libraries and dependencies, so be sure to first enter:

`bower install`

`npm install`

To run the app, simply enter `node basic-server.js` and open the `client/index.html` file with your browser.
Specifically:

- `./server/basic-server.js`
- `./client/index.html`

Make sure to have a valid `config.js` inside the env folder.

### SpecRunner

The SpecRunner contains the tests for the client

### Testing

Tests are written with the [Mocha](https://github.com/mochajs/mocha) testing framework.
They are located in the /spec directory. To run them, enter:

```
npm test
```
