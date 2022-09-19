---
title: "Installing Hugo Site"
date: 2019-06-17T23:53:00+01:00
hideLastModified: true
summary: "How to install Hugo \
on Ubuntu \
and Windows"
tags: ["custom_summary", "code"]
---

**Installation Steps:**


***1. Linux Ubuntu***
   
The official Ubuntu APT repository can be used to directly install the Hugo program.
Update the list of all-apt packages first by opening the terminal window.
Execute the following command to install Hugo using the apt repository in Ubuntu: 

 ***apt-get package***

 sudo apt update 

 sudo apt upgrade 

 sudo apt install hugo 


***2. Windows***
    
 1. Download the latest zipped Hugo executable from [Hugo Releases](https://github.com/gohugoio/hugo/releases)


2. Extract all contects to your *C:\Hugo\bin folder* (the file path can be different depending with your device volume space)

3. Add hugo.exe to *C:\Program Files\System32* (this will allow you to have access of hugo anywhere in your commandline)