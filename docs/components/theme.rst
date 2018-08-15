Themes
======

Themes control the design, look and feel of the website using HTML, CSS, JavaScript, and other front-end assets in order to implement a design for their site. Themes are used to change the HTML markup of anything in Drupal; Add CSS styles to change the layout, color, or typography on one or more pages; and Use JavaScript to enhance the user experience

The theme used is based on Radix which comes packaged with DKAN. Customisations have been done and a new theme (ipbes_new) has been built. The theme uses Gulp_ to compile Sass and check for errors in CSS. Gulp needs Node. This approach minifies the code to make it load fast while simplifying maintenance.

Installation of theme
---------------------

1) Make sure you have Node and npm installed.
You can read a guide on how to install node here: https://docs.npmjs.com/getting-started/installing-node
If you prefer to use Yarn_ instead of npm, install Yarn by following the guide here: https://yarnpkg.com/docs/install.

2) Install bower::

    npm install -g bower

3) Clone the git repository for the webstyles to be next to your project folder::

    git clone https://github.com/ipbes/webstyles.git
    
4) Go to the root of `ipbes_new` theme and run the following commands::

    npm run setup

    To install using Yarn, run::

    yarn install && bower install

5) Configure the destination folder. This is only the source code for the theme and the generated assets need to be
copied to the panthoen repository in the `sites/all/themes` folder::

    export DIST=<pantheon_repo>/sites/all/themes

6) Run gulp to copy the minified styles to the project directory::

    gulp dist
    
Style guide   
-----------
Check the colours here: http://www.color-hex.com/color/81857a

Primary colours
~~~~~~~~~~~~~~~~~~~

- Grey: #676b5e
- Teal: #0a8380
- Teal 50%: #84c2c1;
   - Teal 33%: #aed6d6;
   - Teal 25%: #c2e0e0
- Green: #a5ae60
- Blue: #002e5e

Secondary colours
~~~~~~~~~~~~~~~~

- Greyish green: #81857a
- Purple: #562974
- Orange: #d6490c

    
.. _Gulp: http://gulpjs.com
.. _Yarn: https://yarnpkg.com
