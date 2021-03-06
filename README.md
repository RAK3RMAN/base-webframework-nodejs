# Base WebFramework NodeJS
[![Build Status](https://travis-ci.org/RAK3RMAN/base-webframework-nodejs.svg?branch=master)](https://travis-ci.org/RAK3RMAN/base-webframework-nodejs)

A general template for a Node.js web application running Fastify and Handlebars

### Basic Structure
This project is a base web framework to run a web application using Fastify through Node.js. Being a 'base' framework, this project only displays a webpage through a specified port with no authentication. The structure of this application is described below in the application map.

### Application Map
```
--app.js # Primary NodeJS file
--routes # Routes for views
  --error-routes.js
--templates # Components of webpage, HTML
  --home.ejs # Home Page
  --error.ejs # Error Page
--config # Folder where configurations are set
  --testing.js # Exit options when running in testing environment
  --setup.json # Helper file for config.json
  --config.json # Appears upon system configuration within application
--public # Place static files to be accessed by webpage here
--package.json
--package-lock.json
--start.sh
--LICENSE
--README.md
--.travis.yml
--.gitignore
```

## Install and Setup
- Clone the repository from https://github.com
```
git clone https://github.com/RAK3RMAN/base-webframework-nodejs.git
```
- Setup Base WebFramework NodeJS
    - Enter the base-webframework-nodejs folder
        - `cd base-webframework-nodejs`
    - Install all required packages with root-level access (if needed)
        - `sudo npm install`    
    - Start default application using npm
        - `npm start`
    - If you want a different broadcast port, you can configure these values by proceeding with the:
        - Hardcode option:
            - Enter the `config.json` file
                - `sudo nano base-webframework-nodejs/config/config.json`
            - Edit the `webserver_port` parameter to your desired configuration
    - If any errors occur, please read the logs and attempt to resolve. If resolution cannot be achieved, post in the issues under this project. 
- Access web application through `localhost:3000`
