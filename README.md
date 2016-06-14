

#Gulp guide by Dusan

install nodejs and npm globally

sudo apt-get update
sudo apt-get install nodejs
sudo apt-get install npm

install gulp cli globally

sudo npm install -g gulp
sudo npm install -g bower //bower if needed

==============================
install dependent packages
===============================
first run:

npm install

next create package.json in root folder with:

npm init
==========================
install packages locally for a project from root folder

npm install --save-dev gulp

devDependencies are needed for gulp tasks

--save-dev saves dependencies to package.json

======================
dependencies are needed at runtime (Angular, Bootstrap), npm install --save dependency
or bower install -- save dependency to install and save to

======================

create gulpfile.js in project root, this file contains tasks

gulp utility is a plugin that visibly shows task execution

npm install --save-dev gulp-util

===============================

===============================
use npm to install JS packages

use bower to install Client JS packages

===================

gulp plugins

http://gulpjs.com/plugins/

==============================
gulp recipes

https://github.com/gulpjs/gulp/tree/master/docs/recipes#recipes

======================

jshint and jscs

can be placed in root folder, webstorm can use rules defined by them

WARNING do not use jscs fix option in gulp task, it deletes some stuff from the code!

=======================================
when we have to many requirements it better to load plugins with this:

npm install --save-dev gulp-load-plugins

var $ = require('gulp-load-plugins')

so that we can call plugin like $.jshint without importing it explicitly

=========================================

create reusable configuration module


===============================
list of all tasks

gulp task listing task

=================================

gulp default task

what runs when we type only gulp 

default task can be anything

==================================

compress images with imagemin

compress images
adjust optimization levels

npm install --save-dev gulp-imagemin

==================================================

Build folder - where all the code will be!

=========================================

gulp tasklisting to see names of the tasks

npm install --save-dev gulp-task-listing

=====================================

CSS compiling

less 

*.less -> *.css

automaticaly add vendor prefixes:

====================================
