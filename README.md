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

This will begin tracking all the files in the project directory 

To add the repo to github, you can simply drag the repo's folder onto the  Github for Windows application, and once in there, click on the repo. Now you can click on the "push to github" button in the upper right corner. then again, click on the "Publish" link to make the code available on github. the initial push should be to the Kent Communications github account, and ideally as a "private" repo.


Branches
--------

once you have loaded the project with some initial code, you should create a development branch on the Kent Communications Github

    cd <Project root>
    git checkout -b "Development"
    git push origin Development

now we can fork the development branch to your personal github, and clone this to your local working folder

    git clone git@github.com:<username>/<projectname>.git
    cd <projectname>
    git checkout Development

now create a branch for the feature/bug/change you are going to work on.

    git checkout -b <feature>

now make your changes commit as needed. then push your feature branch back to github.

    git push origin <feature>

now on github go to your personal repo, and go to your feature branch and open a pull request to the development branch on the Kent Communications github. from here, the other members of the team and track your progress and suggest changes, accept yours, or generally discuss the fix/feature/etc.

now the branch can be merged and the development branch will reflect the changes. and once the development branch has been tested and deemed to be ready for primetime, we can pull request the development branch with the master branch and merge them together.


Layout and Structure
====================

Documentation
-------------

a README is vitally important to all repositories, and as such we should make sure they are updated frequently and always reflect the project in it's current state. 

When possible be sure to add a wiki documenting the user's experience in your application/script.

README
------

your readme needs to contain the following information.

### Summary

your readme should begin with a summary of what the purpose of the repoistory is. a Title, and a paragraph giving the general understanding to anyone who opens the repo.

~~~md
Main Project Title
==================

The <Main Project> was created by, <Author Name> to do something really cool, and you should really check out how it is able to do so.
~~~

### Prerequisites

You should explain any tools, libraries, IDEs, runtimes, Operating systems, or applications that are needed in order to run or develop this application.

You should have a bulleted list of applications that are needed (with links when possible.)

~~~md
### Required applications

* [Scite for AutoIt](autoit.com)
* [BCC Mail Manager](bellhowell.net)
* [SQLite](sqlite.org)
~~~

### Setup

The most important portion of any README is this section. Here is where you explain how to get a workstation setup to begin developing and ready to make code changes. 

#### Workstation Configuration

You should be sure to explain how to configure all of the programs that differ from the standard or default installation. 

##### Databases

You need to have instructions on how to setup a database for use with your application, because we shouldn't track the databases in version control, this is a vital portion of setup, here we need to be very clear about how to setup the database. so that from scratch a new instance could be created to run the application on another machine. 

##### Mapped drives / Paths

We need to ensure that our code is made general and able to run on any machine (even one not on our network) so we need to note any paths used either in the code, or utilized via mapped drives, etc. To begin with, simply make note f the places and paths that will need to be updated, and where the user/developer might need to point them (or what they are used for).

We want to make it so that a new user could use this document to get a working development workstation runnig without any other user intervention. 

### 

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


### Data


### Tests


### .gitignore


Install Script
--------------



Intermediate steps
------------------

- Databases
  - track in DB
only until an install script or instruction are availble to create a local instance.

VBA code should be stored in Source files in their own sub dir when possible.
