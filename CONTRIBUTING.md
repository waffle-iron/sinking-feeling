
Note this project is for team members of the Penn State Software Enginnering 500, Summer 2016, Team 5 group. If you are not one of those team members, any pull requests, bug reports, etc will be rejected until the end of August, 2016. 

Repositories
============

There are going to be several levels of source control in use. 

Starting at the top will be the main repository's "release" branch. This is the code that will run on the production web server. Assuming we can get everything working correctly, when we merge to this branch, it will automatically go to the web server and become live.

The next level down will be the main repository's "develop" branch. This should be similar to master, except instead of automatically going to the production server, it will go to the development server. Anything that goes into the release branch must go through here first as the only way to merge to the release branch is to merge from develop. The way to get changes into the develop branch is to submit a pull request and have the maintainer accept that request.

The last level is each user's individual repository. This is where we write our code and put in fixes and it must be a fork of the main repository. The recommended method of operation is to never make commits to the release or develop branches, instead for each item that you write, create a branch off of an up-to-date copy of the develop branch (see below for how to keep your copy of develop up to date) make your change there and submit a pull request from that branch to the master repository's develop branch.

To keep your copy of release and develop up to date, each user should add a second remote to the repository on their computer. By default, when you clone, the place you cloned from is added as a remote called 'origin'. You can add another remote (call it something like 'group') and make your release and develop branches track that instead of your forked repository.
