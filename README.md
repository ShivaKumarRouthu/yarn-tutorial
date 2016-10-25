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
- reliable
- consistent
- offline download

##### Speed

The speed is the one of the major issue resolved by yarn over npm. Yarn will download all the package and dependency packages asynchronous that is how the yarn will download the packages and maintain same architeture like npm.

``````
npm install 
``````




