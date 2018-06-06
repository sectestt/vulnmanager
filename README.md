# vulnmanager

[![Build Status](https://travis-ci.org/xebia-research/vulnmanager.svg?branch=develop)](https://travis-ci.org/xebia-research/vulnmanager)

#### This is a vulnerability manager with an authenticated API to manage vulnerability reports in a webGUI.

__We currently support the following scanning tools:__ 
 * [x] Nmap
 * [x] OpenVAS
 * [x] OWASP ZAP
 * [x] Clair
 
#### Report formats 
The vulnmanager parser currently supports the following report formats per scan tool:

 | Scanning Tool | Report Format | 
 | ------------- | ------------- |
 | Clair | JSON |
 | OpenVAS | XML |
 | ZAP | XML & JSON |
 | Nmap | XML |


## Dependencies:
 * Docker
 * Npm 5+
 * nodeJS 8+
 * Postgresql 10
 * Maven (Maven can download the rest of the dependencies with __mvn install__)
 * AngularCLI
## Installation:
Everything is run in docker, for your convenience ! :whale:

1. Make sure the dependencies are installed (or run __sudo ./dependency_install.sh__)
2. Git Clone this repo
2. Run __./install_docker.sh__ to automagically pull, build and compose the necessary docker containers. 

Currently, there is a basic Angular5 webGUI available by running:
1. __npm install @angular/cli__
2. __cd__ to GUI folder inside git project
3. __npm install__
4. __ng serve --open__
