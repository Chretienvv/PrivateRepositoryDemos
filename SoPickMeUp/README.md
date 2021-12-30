<p align="center">
  <a href="https://angular.io/">
    <img src="https://www.angularexampleapp.com/assets/images/angular.svg" alt="Logo" width=72 height=72>
  </a>

  <h3 align="center">Angular Sopickmeup</h3>

  <p align="center">
   Sopickmeup web-app with Angular 8
    <br>
    <br>
    Base project made with much :heart:. So Pick Me Up is a carpool App, mainly aimed at Sogeti events!
    <br>
    <br>
    <a href="https://sopickmeup.herokuapp.com/">LIVE DEMO</a>
    <br>
    <a href="https://sopickmeup.herokuapp.com/">
      <!-- <img src="https://media.giphy.com/media/ce28l1P13CVK56OyCN/giphy.gif" alt="Demo example"/> -->
    </a>
  </p>
</p>

## Table of contents

- [What's included](#whats-included)
- [Code and branches](#code-and-branches)
- [Setup FrontEnd Mac](#setup-frontEnd-on-mac)
- [Setup FrontEnd Windows](#setup-frontEnd-on-windows)
- [Architecture](#Architecture)



<!--## What's included-->

<!-- - [x] Use of [preboot](https://github.com/angular/preboot) module to share state between browser and server -->
<!-- - [x] Lazy loading images with [ng-lazyload-image](https://github.com/tjoskar/ng-lazyload-image) -->
<!--- [x] Flex positioning-->
<!--- [X] Bootstrap elements / Responsive layout-->
<!--- [x] SASS (most common used functions and mixins) and BEM styles-->
<!-- - [x] Scroll to first invalid input in forms. ([ngx-scroll-to-first-invalid](https://github.com/Ismaestro/ngx-scroll-to-first-invalid)) -->
<!--- [x] ES6 Promises and Observables-->
<!--- [x] Unit tests with Jasmine and Karma.-->
<!--- [x] Backend on a seperate gitlab reposetory : https://gitlab.sogeticloudservices.com/chretien.van.veldhuizen/pick-me-up.git-->




### Code and branches
<p>In this section some rules/tips about how to write code in sopickmeup is written. </p>
<ol>
    <li>We do the following for branch naming:
        <ol>
            <li>For bugfixes we use "bugfix/nameofthebranch"</li>
            <li>For features we use "features/nameofthebranch"</li>
            <li>For tests we use "test/nameofthebranch"</li>
        </ol>
    </li>
    <li>In the microsoft teams wiki tab is information about how your code should be written. For example: how to name functions.</li>
    <li>The project uses Sass BEM method in a different map folder than the default component style sheets that angular creates.</li>
    <li> We use bootstrap</li>
</ol>


## Setup FrontEnd on Mac
<p>This chapter will walk you through installing the essentials for the FrontEnd. There is a setup for Mac, Windows and Linux. This will provide the Mac version </p>
<p> Mac setup. </p>
<p><b>Installing homebrew, Node.js, NPM and Bootstrap</b></p>
<p>We will be using this link <a href="https://treehouse.github.io/installation-guides/mac/homebrew">"How to install homebrew"</a></p>
<ol>
    <li>Go to the app store and install Xcode. This is needed for Homebrew. If this is installed go to step 2</li>
    <li>Open the recently mentioned link. In this link the installing steps of homebrew are explained. We will also explain them here for further clarity. </li>
    <!--Check deze link nog ff-->
    <li>Open the terminal on your Mac and copy paste the following command: $(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install). If homebrew is installed go to step 4</li> 
    <li>To install Node.js and Npm type the following command in the terminal: brew install node . 
    <br></br>To check if Node is installed type the following command: `node --version` . If the result is v12.13.1 or higher then congratulations you now have Node.js.
    <br></br>To check if Npm is installed type the following command: npm --version . If the result is v6.12.1 or higher then congratulations you now have Npm.
    </li>
</ol>
<p><b>Installing Angular on Mac</b></p>
<p>For this section we will be using the following link <a href="https://cli.angular.io/"> "How to install Angular"</a></p>
<ol>
    <li>Type the following command in your terminal: npm install -g @angular/cli . 
    <!--Check of deze command werkt ng --version-->
    <br></br>To check if Angular is installed type the following command: ng --version . If the result is version 8 or higher then congratulations you now have Angular installed. </li>
</ol>
<p><b>Cloning the repository of so-pick-me-up to your editor</b></p>
<ol>
    <li>To clone the repository of so-pick-me-up use the following command: not for you ;) 
    <br></br>
    Navigate to the sopickmeup folder in your terminal to open the files in your editor.
    </li>
    <li>We use Tslint as our linter. In your editor extensions search for tslint and install it.</li>
    <li>You are now able to work on sopickmeup</li>
</ol>


## Setup FrontEnd on Windows
<p>This chapter will walk you through installing the essentials for the FrontEnd. There is a setup for Mac, Windows and Linux. This section will provide the Windows version </p>
<p> Windows setup </p>
<p><b>Installing Node.js, Npm, Angular and Bootstrap</b></p>
<ol>
    <li>Go to https://nodejs.org/en/download/ and download node.js windows installer. </li>
    <li>Run the installer if you completed the installer steps go to step 3.</li>
    <li>Restart your computer if this is done go to step 4.</li>
    <li>To check your version of node.js open the terminal and type the following command node --version. Make sure to have version 12.13.1 or higher</li>
    <li>To check if Npm is installed type the following command: npm --version . If the result is v6.12.1 or higher then congratulations you now have Npm.</li>
</ol>
<p><b>Installing Angular on Windows</b></p>
<p>For this section we will be using the following link <a href="https://cli.angular.io/"> "How to install Angular"</a></p>
<ol>
    <li>Type the following command in your terminal: npm install -g @angular/cli . 
    <!--Check of deze command werkt ng --version-->
    <br></br>To check if Angular is installed type the following command: ng --version . If the result is version 8 or higher then congratulations you now have Angular installed. </li>
</ol>
<p><b>Cloning the repository of so-pick-me-up to your editor</b></p>
<ol>
    <li>To clone the repository of so-pick-me-up use the following command: not for you
    <br></br>
    Navigate to the sopickmeup folder in your terminal to open the files in your editor.
    </li>
    <li>We use Tslint as our linter. In your editor extensions search for tslint and install it.</li>
    <li>You are now able to work on sopickmeup</li>
</ol>



### Architecture
<h5>1. Component structure</h5>
<p>Views are divided into components. These components can be found in 2 places:

- app>shared>components: These components are not linked to a certain page/functionality of the app. Example: banner, 404 page
- app>modules>*>components: These components are linked to a certain functionality or page of the app. This page/functionality has its own module so these components are grouped together

Generally views should be split into multiple components if it improves readability of the code or if a certain part of the view is going to be reused.
</p>

<h5>2. Services</h5>
<p>
The services can be found in the app>core folder. There are currently 2 types of services:

- normal services: Their main function is to pass data to the components. Usually these are retrieved from an Api.
- guards: These can prevent access to certain components. This is used for authorisation.

When making api calls, it is preferable to use the helper functions in api.service.ts. The functions in this service make sure the correct URL is used and add the necessary headers.
</p>

<h5>3. Modules</h5>
<p>
The modules in the app have multiple functions.<br>
Firstly, there are the modules found in the app>modules folders. These generally refer to a specific page in the app, and handle the imports, exports and declarations for the components that are used in that page.<br>
Secondly, there are the routing modules. These are also found in the app>modules folders. These handle the routing for the different pages.<br>
Thirdly, there are modules for the other functionalities in the app: core.module and shared.module. These make sure the shared components and services are declared and provided.<br>
Finally, there is the app.module. This module handles the imports, exports, declarations and providers for the whole app. In order to keep this file clean, most of the responsibilities have been delegated to the other modules.
</p>

<h5>4. Folder structure</h5>
<p>
The SoPickMeUp folder structure follows a similar principle to the folder structure [here](https://itnext.io/choosing-a-highly-scalable-folder-structure-in-angular-d987de65ec7)
</p>

<h5>5. Environments</h5>
<p>
There are 3 environments:

- Dev: The app uses the api at localhost:8080, the developer should install and run the sopickmeup back-end from not for you
- Test: The app uses the api hosted on a public heroku server
- Prod: The app uses the api hosted on Sogeti's AWS server

</p>


Tasks                       | Description
----------------------------|---------------------------------------------------------------------------------------
ng serve                    | Start the app in development mode with the english language only
ng test                     | Run the unit tests
ng serve --configuration=test | Start the app for the heroku test environment
npm run server              | Start the app in production mode

<!-- add commands for aws server methods -->

### Optional: SonarCube 
<!--Needs an expansion on installing sonarQube -->
Run this command from project root to run a new SonarQube analysis.

Download sonarqube and replace the projectkey and login with your own!

`sonar-scanner \
  -Dsonar.projectKey=sopickmeup-frontend \
  -Dsonar.sources=. \
  -Dsonar.host.url=http://localhost:9000 \
  -Dsonar.login=1c664caa413bc11ad03b8345f84865e41502bab0`
