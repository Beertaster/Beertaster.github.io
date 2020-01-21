---
layout: post
title:      "Module Project 1: Web Scraper"
date:       2020-01-21 00:16:37 -0500
permalink:  module_project_1_web_scraper
---


This project is a culmulation of the object oriented lessons of the previous month. The challenge is to create a program that will loop a series of if statements to create command line interface (CLI) menu from which the user can initiate the different functions of the Web Scraper.

For this assignment I chose Axios.com as my source of scraped information. Axios is a news site that specializes in giving more concise news stories which can be expanded upon pressing a button. The site actually has the expanded information loaded with the rest of the website and listed as hidden. So I wanted my scraper to also grab the hidden part of the articles as well, and like the site itself, also  have an optional command to show the expanded news story in the scarpper's main menu.

While the CLI contains the most lines of code it is straightforward and simple to create. So I decided to search for a way that could spruce up the presentation of the printed menu lines to be more aestetically pleasing. I found extra formatting commands like .blue and .bond which could add emphasis to the cli.

https://assets-cloud.enjin.com/users/1654670/pics/original/4144927.jpg

Second, the news.rb portion of the scrapper is a more standard object class to hold the information that the nokogiri plugin would return. Each time Nokogiri sends a group of values, the class creates an object instance and ties it to an array. Its not much different then what's in most lesson's up to this point so I would like to focus on nokogiri itself.

https://assets-cloud.enjin.com/users/1654670/pics/original/4144928.jpg

Nokogiri is a web plugin that was make to take in an internet address and output a number of html segments as string variables. An easy method of configuring nokkogiri is by writing a bit loop to grab iterate over every instance of a reoccuring html box or division that contains several pieces of relevant information. headers, paragraphs, links and more will be turned into strings and set to a variable. Lastly the loops sends those new values to create a new instance of an object.

![](https://assets-cloud.enjin.com/users/1654670/pics/original/4144929.jpg)

From here the CLI lists the News title of each story in a menu for the use to pick from, until the user types exit.
