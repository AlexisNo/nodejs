Node.js docker image for development environment
================================================

Not maintained

A Docker Node.js image with some useful packages for development environments.
Do not use it for production.


Configuration
-------------

Globally installed npm packages:

 * forever
 * yo (yeoman)
 * bower
 * gulp
 * grunt-cli
 * node-inspector


Common usage
------------

This image should be used as a basic image for any project.

 * Create a Dockerfile based on this image and add your project dependencies.
 * Create you own image with `docker build` or `docker-compose build`.

Run your new image with a command similar to this:

    docker run -d -p 80:80 -v /path/to/your/project/sources:/var/www/project-name
