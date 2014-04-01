KCI Programming Projects
========================

Before you begin
----------------

If the project you are starting is in fact new, start by creating a repo on github. Otherwise you should initialize a git repo in the existing codebase and add that to github.

New Projects
------------

Go to the [Kent Communications Github page](http://github.com/KentCommunications/) and click on the "New Repository" button to create your repository.      

Existing Projects
-----------------

Open a shell in the root of the project directory and run the following commands:

    > git init     
    > git add --all
    > git commit -am "Initial Commit"

This will begin tracking al the files in the project directory 

Layout and Structure
====================

Documentation
-------------

wiki when possible. except intial setup and need to know before editting and submitt patches, which should be in the README.md

Code
----

### Directories

#### top level 

* Source
  * all source files
  * lib folder 
    * contains all thirdparty libraries, or UDFs
* data
  * testing data
  * access databases
    * must contain any needed VBA
* tests

#### root dir

* .gitignore
* README.md
  * How to setup initially
    * Begin development
    * run first job
    * submit patch
  * Who started the project
  * any outstanding bugs
  * need to know info
* install script

SOURCE
-----


Data
----


Tests
-----


.gitignore
----------

README.md
---------

Install Script
--------------



Intermediate steps
------------------

- Databases
  - track in DB
only until an install script or instruction are availble to create a local instance.

VBA code should be stored in Source files in their own sub dir when possible.
