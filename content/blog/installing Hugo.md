---
title: "Installing Hugo Site"
date: 2019-06-17T23:53:00+01:00
hideLastModified: true
summary: "How to install Hugo \
on Ubuntu \
and Windows"
tags: ["custom_summary", "code"]
---

# **Installation Steps:**


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

# Now lets install our first hugo site.

NB: [Hugo Themes](https://themes.gohugo.io/themes/) we are going to choose hugo-refresh the one i am currently using:


# Create site and cd into it
hugo new site my-site && cd my-site

# Clone the ReFresh theme into the themes folder
git init
git submodule add https://github.com/PippoRJ/hugo-refresh.git themes/hugo-refresh

# Remove the default config
rm config.toml

# Fetch the example config
curl -O https://raw.githubusercontent.com/PippoRJ/hugo-refresh/master/exampleSite/config.yaml

# Run the site locally
hugo server -D

# Open the site in your browser
open http://localhost:1313

To run the Example Site using Hugo ReFresh:

# Create site and cd into it
hugo new site my-site && cd my-site

# Clone the ReFresh theme into the themes folder
git init
git submodule add https://github.com/PippoRJ/hugo-refresh themes/hugo-refresh

# Remove the default config
rm config.toml

# Copy the Example site content and configuration in my-site
cp -R themes/hugo-refresh/exampleSite/* ./

# Open the site in your browser

hugo server -D


![image alt text](/images/hug.png)