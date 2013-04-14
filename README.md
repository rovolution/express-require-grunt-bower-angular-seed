### express-require-grunt-bower-angular-seed 
---
# the seed for AngularJS apps (on steroids)

Apart from it's amazing name, this particular angular seed application provides a good starting point for building an application that includes:

 1. [grunt.js](http://gruntjs.com/)
 2. [bower.js](https://github.com/twitter/bower)
 3. [require.js](http://requirejs.org/)
 4. [express.js](http://expressjs.com/)
 5. [jade](http://jade-lang.com/)
 5. [angular.js](http://angularjs.org/)

## Requirements

 1. node
 2. npm 
 3. grunt.js
 4. bower.js

## How to use

Follow these simple steps to get you started and up to date:

 1. clone the project
 2. install node dependencies  
    __npm install__
 3. install bower dependencies  
    __bower install__
 4. run the tests  
    __grunt test__
    
## Build step

This application seed (with his amazing name, if i might add). Provides a build step to build a minimised and concatenated javascript with the amazing [r.js](https://github.com/jrburke/r.js/) tool.

To run the build step simply run __grunt build__. 

### What does it do?

The build step contains of three major steps

 1. all files and folders from __public__ will be copied to __public-app__
 2. require.js library is uglified
 3. r.js tool is started on __main.js__ to concatenate and uglify require modules.
 
 
### How does a built app look like?

The built application (emu, actually, public folder) contains all the files as the current public folder.

However the built application concatenates all require.js modules to one file named as __main.js__ (source maps will be provided, oh joy!).

## Testing

This amazing seed project provides the user with three different type of tests:

 1. e2e tests for client side
 2. spec tests for client side
 3. spec tests for server side
 
grunt jobs for tests:

 1. grunt test  
    * spec tests for client side
    * spec tests for server side
 2. grunt test:e2e
    * e2e tests for client side
 3. grunt test:spec
    * spec tests for client side
 4. grunt test:all
    * RUN EVEEERYYYTHINNNGG!!!