# email2spark

A simple program that will move an email thread to a Cisco Spark room using www.mailgun.com

## Setup
* Create an account on mailgun.com and validate the domain you are going to use.  
* Clone this repository and install the dependencies by running 'npm install'
* Setup your enviroment variables (SEE below)
* Create an new route for yourbotname@yourdomain.com on mailgun.com that triggers a oubound webhook to the url of this application (http://app.domain.com:3000/mailgun)
* run the app

## Enviroment variables

* export MAILGUN_API_KEY='key-xxxxxxxxxxxxxxxxx'
* export DOMAIN='yourdomain.com'
* export PORT=3000
* export BOT_EMAIL='yourbotname@yourdomain.com'
* export BOT_ID='yourbotname@sparkbot.io'
* export BOT_ACCESS_TOKEN='YOURBOTACCESSTOKEN'

## Usage

After the application is setup.  All the user has to do is reply all to the email thread and BCC yourbotname@yourdomain.com.

