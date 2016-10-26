# Yarn-tutorial

The new era of package manager has just started with npm and it has changed the way of managing the packages. It has pro's and con's . Now comes the new package manager called yarn that overcomes the problems in npm and establish a new benchmark for the 
packages installation.

## Introduction

It is a new package manager introduced by facebook. This was build to overcome issues like consistency, speed etc.. Using this manager we can do more than what can be done using npm. internally yarn will be pointing same repository that npm does but the only difference is the implementaion.

Yarn does things by using concept of caching and asynchrounous package downloading. Yarn will download packages 4X times faster than npm. It can download the packages offline too. 

## Setup Yarn 

``````
npm install -g yarn
``````
Type yarn in terminal / command prompt
``````
yarn install v0.16.1                                                                               
success Already up-to-date.                                                                  
Done in 0.25s.
``````

you can find other ways of installations [here](https://yarnpkg.com/en/docs/install#mac-tab)

### Features of Yarn

- speed
- reliable & consistent
- offline download

##### Speed

The speed is the one of the major issue resolved by yarn over npm. Yarn will download all the package and dependency packages asynchronous that is how the yarn will download the packages and maintain same architeture like npm. Consider package.json with few packages already added to this repository and give following two commands and see how much time they takes

``````
npm install 
``````

``````
yarn
``````
##### Reliable

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Yarn takes care of full installation of node modules on different operating systems. It uses the detailed description of each node module in the lockfile to guarantee installation on different operating system with consistency.

##### Offline Download

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Yes.. yarn can download the packages in offline mode if you have installed the package in your machine atleast once. use below command to install a package offline 

``````
yarn install socket.io --offline
``````



## Commands 

* init
* install
* add
* update 
* remove
* config


**yarn init** 
This is similar to npm init, it will initialize a package with few question and create a lockfile. A lockfile is similar to shrinkwrap in npm to maintain consistency over downloading node modules



**yarn install** or **yarn** 
This is similar to npm install, it will download all the packages from package.json file and update the same in lockfile. During *migration* from npm to yarn use same command on existing package.json file to download node modules resolving dependencies and create a lockfile. yarn install can be used with different flags --offline, --force, --flat, --production and other .. [Read more](https://yarnpkg.com/en/docs/cli/install)


**yarn add (package name)@(version number)**
This will download the node module specified and add them to the package.json and yarn.lock file.
``````
yarn add express@3.0.0
``````

**yarn upgrade (package name)@(version number)**
This will download the node module specified and updated them to the package.json and yarn.lock file. If you do not specify any package name it will automatically upgrade all the packages from package.json
``````
yarn upgrade express
``````


**yarn remove (package name)@(version number)**
This will remove the node module specified and also remove them from the package.json and yarn.lock file.
``````
yarn remove express
``````

**yarn config**
This is used to view/set the configuration of yarn.

To view full configuration
``````
yarn config list
``````

To set an configuration propety of yarn
``````
yarn config set <key> <value>
`````
[additinal information of commands can be found at this link](https://yarnpkg.com/en/docs/cli/)



