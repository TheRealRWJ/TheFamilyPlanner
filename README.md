# TheFamilyPlanner
Webpage driven Family planner



# The Family Planner  

## Description A monitor displaying dashboard displaying I.e. 

the family schedule privacy driven content using your own Nextcloud instance in stead of something like Google Scraping pages with i.e. Beautifulsoup in stead of using APIs and online accounts  

## Requirements  

### Hardware Part 
1. A 'server' running Nextcloud and a light weight web server Part 
2. A Raspberry Zero with a monitor loading the web page in kiosk mode Part 
3. Smart Phones of family members filling calendars, tasks and lists synced to the Nextcloud instance Part 
4. A simple small remote or gamepad to navigate the pages on the monitor.  

### Software Linux 
> Some light function like raspbian  
Nextcloud (With an extra user for shared content) 
> Nextcloud is available as a snap  
A lightweight web server with static pages Python 
scripts ran by cron jobs populating json files JavaScript injecting content of webpage from the json files to prevent page refreshes 
A separated settings file with preferences and hyperlinks readable by human and Python  

> I use DAVx5 to sync my nextcloud calendars to my phone  

> KDE-Connect mouse function for navigating   

## The webpage  privacy driven Locally created content  
A responsive CSS driven website viewable on multiple device types (Monitor, tablet, phone) i.e.  using bootstrap blocks 

I think current version look pretty neat on the desktop or tablet But it sucks on a phone  

### The page content could be 
1. A menu with simple icons populated by a json file displayed on all pages  
1. Revolving background images from specified  folder 
1. Actual date and time 1. Actual weather info  
1. A combined calendar of all family members. first up event enlarged on top 
2. A grocery list split in food and no food 
3. Task list 
4. Todo list 
4. Other plugins possible on different pages  

## Plugins 
Plugins are modular Plugins have there own page, Python script json file and JavaScript 
similar plugins could share a single page 
Pages should still be up when plugins fail to load
