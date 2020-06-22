---
layout: post
title:      "Project 2 - Sinatra Site"
date:       2020-06-08 04:44:39 -0400
permalink:  project_2_-_sinatra_site
---

Assumptions are the bane of all programming. Assuming to know how a route, rack command, or any library method that been imported to a project works is a great way to spend a few hours banging ones head against the wall. That unfortunately is the story of this project. I had several assumptions about my knowledge of the material, which all highlighted missing knowledge from the curriculum. Thankfully completing this project has forced me to realise my gaps in knowledge, unfortunately that happened by deciphering error messeges. For example.

I completely overlooked the fact that the restful routes PATCH, DESTROY, and PUTS require 'use Method:override' in the config file to modify tables. With this in mind updating edit was as simple as adding 

'@post.update(title: params[:title], review: params[:review], rating: params[:rating])'

to the patch route after having got the '@post' in question from the helper method.

I also had some issues in the beggining using VS Code. That was more that I hadn't used it in a long time and wasn't familiar with commands.

Learning from errors is memorable, but slow, frustrating, and an inevitability for anyone that hasn't coded larger projects in some time. However, it did work to drill down best practices into mind, re-teach me the mentality to problem solve code. To look for typos, to avoid typos, to read error messages and back trace to where the issues are, and comfirm as to whether or not I have complete understanding of how an code functions.

Below are some notes that I wrote while doing the project which outline my frustrations and some times cluelessness about what is happening in my code.
_________________________________________________________

I found the most difficult part to be not the building of the site, but implementation. Most of the Sinatra site is structured by MVC and restful routes. These are more or less best practices that minimize the amount of coding needed and makes the code easier to understand by others, through its organization. 

I didn't think I'd find myself stuck in Visual Studio Code because I didn't realised I messed with my terminal and now it wouldn't read anything from the whole project. Or when I upload my project to Github and for some reason it won't take my db folder and all the files I generated inside. I still need to ask about that.

I kind of forgot that getting to the point that I can tinker and reload my project over and over isn't a given and everything has to be set up right

When I was using rake migrations I assumed that I could migrate over old information and realised that the 3 commands I had been using over and over to migrate, set the env of dev and test to be the same, and end pending migrations. I hadn't saved the changes I made to the generated tables and got a crash course in how and when rake databases update. It caused me to scrap a lot of schemas but I read up on rake commands and how each one specifically works.

Its been one thing after another writing this project. I realize why my rake migration files aren't updating the schema because they havn't been induvidually saved. Then when I do have a correct migration, my from page breaks down. I get error messages that says no method for 'username' in --><h2> <%= current_user.username %></h2>-- when this has been there from the start and always worked. I didn't even change the users migration file its located in. I changed the posts file to incorporate more stored variables per object.

The signup page works though. Unfortunately adding editing functionality broke the whole thing I got more boot errors.

.
