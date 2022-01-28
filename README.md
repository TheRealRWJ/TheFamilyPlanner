# The Family Planner
Privacy driven Family planner

## Description 
A monitor displaying a dashboard showing I.e. the family schedule   
Privacy driven content using your own Nextcloud instance instead of something like Google  

## Requirements  

### Hardware requirements 
1. (access to) A 'server' running Nextcloud and a light weight web server 
2. 1.e. A Raspberry Zero with a monitor loading the web page in kiosk mode Part 
3. Smart Phones of family members filling calendars, tasks and lists synced to the Nextcloud instance  
4. A simple small remote or gamepad to navigate the pages on the monitor.  

### Software 
1. Linux 
> Some light function like raspbian  

2. Nextcloud, with preferably an extra user for shared content so the wabpage has no access to your own account.

3. A lightweight web server with static pages 

4. Python 
scripts ran by cron jobs populating json files JavaScript injecting content of webpage from the json files to prevent page refreshes 
5. App to sync Nextcloud calendars and lists with phones
> I use DAVx5 to sync my nextcloud calendars to my phone  

> KDE-Connect mouse function for navigating   

### The webpage  
privacy driven Locally created content  
A responsive bootstrap driven website viewable on multiple device types (Monitor, tablet, phone) 
I think current version looks pretty neat on the desktop or tablet But it still sucks on a phone  

### The page content could be 
1. A menu with simple icons populated by a json file displayed on all pages  
1. Revolving background images from specified folder 
1. Actual date and time 1. Actual weather info  
1. A combined calendar of all family members. First up event enlarged on top 
2. A grocery list, Task list, Todo list 
4. Other plugins possible inthe future on other pages  

## Plugins 
Plugins are modular Plugins have there own page, Python script json file and JavaScript.  
Similar plugins could share a single page  
Pages should still be up when plugins fail to load  
Still needs a lot of work.


## To Do
Read settings from file
Fix layout on small screens
  - Order of content needs to be changed, so more important info resides on top of the page
Enable plugins
Get data from necxtcloud in a secure way. Dont like current usage of public calendars and tasks
Get picture of planned meals out of mealy 

By the way I only dabble in python, javascript and html/css
