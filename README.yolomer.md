yolomer
=======

## Contents
  * [README samples](README.md)
  * [Setup](#setup)


## About Yolomer

There are many ways to get started scaffolding a Polymer project, including the use of [Yeoman](http://yeoman.io/) which just acquired its very own [generator-polymer](https://github.com/yeoman/generator-polymer) project, maintained by the [Chrome Developer Relations](https://github.com/yeoman) team.

 Watch [Rob Dodson's](https://github.com/robdodson) video guide to Yolomer.

<a href="http://www.youtube.com/watch?feature=player_embedded&v=INH_OW4lFSs" target="_blank" align=center>
<img src="http://img.youtube.com/vi/INH_OW4lFSs/0.jpg" alt="YOLOmer! Polymer and Yeoman for lighting fast dev" 
width="250" border="10" /></a>


## Setup

The following was built/tested on a MacBook Air running OS X (version 10.0.4). [YMMV.](http://en.wiktionary.org/wiki/your_mileage_may_vary)


Install [Node Package Manager (npm)](https://github.com/npm/npm) if you haven't already done so. It now comes standard with [Node.js](http://nodejs.org/) and is a must-have tool for any serious web app developer. _We will use npm to bootstrap our Yeoman installation._

Install [Bower (bower)](http://bower.io/) for package management and [Grunt](http://gruntjs.com/) for build management if you haven't already done so. While its possible to use other packages for these needs, the  prescribed [Yeoman workflow](http://yeoman.io/assets/img/workflow.1bf8.jpg) shows this to be the most effective way to go.

Install [Yeoman (yo)](http://yeoman.io/learning/) if you haven't already done so. It is a web app scaffolding tool that has 'generators' (seed configurations) for various web app platforms. It is [maintained by](https://github.com/orgs/yeoman/people) members of the Chrome Developer Relations Team and others. 

```
npm install -g yo
```

Install [generator-polymer](https://github.com/yeoman/generator-polymer) also using npm.

```
npm install -g generator-polymer
```

Now create your directory for the new polymer project, cd into it, and scaffold out a new polymer project.

```
mkdir -p yolomer && cd $_
yo polymer
```
This should scaffold a _complete_ Polymer app. (Note that [other Polymer generators](https://github.com/yeoman/generator-polymer#generators) exist for other purposes.

The Yo scaffolding process asks a number of questions to configure your boilperplate. I stuck to defaults.

```
[?] Would you like to include core-elements? Yes
[?] Would you like to include paper-elements? Yes
[?] Would you like to use SASS/SCSS for element styles? Yes
[?] Would you like to use libsass? Read up more at 
https://github.com/andrew/node-sass#node-sass: No

 ..
 ..

I'm all done. Running bower install & npm install for you to install the required dependencies. If this fails, try running the command yourself.
```

Once the project is scaffolded out, you should see the following structure in that directory.

```
.bowerrc
.editorconfig
.gitattributes
.gitignore
.jshintrc
.yo-rc.json
Gruntfile.js
app
bower.json
node_modules
package.json
```

## Run

If all is well, you should now be able to run the simple web app using

```
grunt serve
```

This should run a local server hosting your web app, and launch a browser pointing to the default port on which the app is served. The result should look something like this.

![](img/yolomer-1.png)

Congratulations. Your yolomer scaffolding works. Now onwards into exploration!


## Explore