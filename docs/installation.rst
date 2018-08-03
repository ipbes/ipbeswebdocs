============
Installation
============
The code for the site is based on DKAN. The code is hosted on pantheon.io and available only to members.
Install the package with pip::

    $ pip install read-the-docs-template
    
============
Installation for web styles
============

The IPBES theme uses [Gulp](http://gulpjs.com) to compile Sass. Gulp needs Node.

Step 1
-----------------
Make sure you have Node and npm installed.
You can read a guide on how to install node here: https://docs.npmjs.com/getting-started/installing-node

If you prefer to use [Yarn](https://yarnpkg.com) instead of npm, install Yarn by following the guide here: https://yarnpkg.com/docs/install.

Step 2
-----------------
Install bower::

    npm install -g bower`.

Step 3
-----------------
Go to the root of `ipbes_new` theme and run the following commands: `npm run setup`.

To install using Yarn, run::

    yarn install && bower install

Step 4
-----------------
Configure the destination folder. This is only the source code for the theme and the generated assets need to be
copied to the panthoen repository in the `sites/all/themes` folder::

    export DIST=<pantheon_repo>/sites/all/themes

Step 5
-----------------
Run::

    gulp dist`    
    
    
