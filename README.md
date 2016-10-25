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

Yarn takes care of full installation of node modules on different operating systems. It uses the detailed description of each node module in the lockfile to guarantee installation on different operating system with consistency.

##### Offline Download

Yes.. yarn can download the packages in offline mode if you have installed the package in your machine atleast once. use below command to install a package offline 

``````
yarn install socket.io --offline
``````








