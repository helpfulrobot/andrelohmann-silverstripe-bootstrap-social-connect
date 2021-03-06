# bootstrap_social_connect

## Maintainers

 * Andre Lohmann (Nickname: andrelohmann)
  <lohmann dot andre at googlemail dot com>

## Requirements

Silverstripe 3.2.x

## Introduction

Social Login/Connect with Twitter, Facebook and Google

## Usage

Set AppID Parameters like in _config.php

The signup methods on FacebookController, TwotterController and GoogleController are just examples.
Write your own Signup Method (with your specific form and parameters) and set the pathes.

### Create Apps

#### Facebook

 * go to https://developers.facebook.com/apps/ and create a new app
 * set the correct URL
 * fetch API Key and API Secret and set inside your _ss_environment.php

#### Google

 * go to https://console.developers.google.com/project and create a new Project
 * enter the new project and go to APIs
 * remove every API except (or add) Google+ API
 * go to credentials/Zugangsdaten and add an OAuth Client ID

#### Instagram

 * go to https://instagram.com/developer/ and register your application (Manage Clients)
 * set the correct URL
 * fetch API Key and API Secret and set inside your _ss_environment.php

#### Twitter

 * go to https://apps.twitter.com/ and create a new application
 * set all necessary URLs and save
 * go to settings and check "Allow this application to be used to Sign in with Twitter"
 * copy all credentials

### Sources

used following sources for implementation

Facebook Login

https://developers.facebook.com/docs/facebook-login/login-flow-for-web-no-jssdk/

Google Login

https://developers.google.com/+/web/signin/server-side-flow
https://developers.google.com/accounts/docs/OAuth2WebServer

Twitter login

https://dev.twitter.com/docs/auth/implementing-sign-twitter
https://dev.twitter.com/docs/auth/oauth

https://github.com/abraham/twitteroauth

### Notice
This repository uses the git flow paradigm.
After each release cycle, do not forget to push tags, master and develop to the remote origin
```
git push --tags
git push origin develop
git push origin master
```