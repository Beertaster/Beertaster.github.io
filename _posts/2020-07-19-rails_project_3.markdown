---
layout: post
title:      "Rails Project 3 "
date:       2020-07-20 00:07:14 +0000
permalink:  rails_project_3
---


Authentication and verification have been a source of bloat in all my projects. Even writing helper methods to lower the number of necessary line of code to try and fool proof code against tampering. It often end up being half the code on some pages.

At least has_secure_password and Omni_auth don't require much coding to set up. In fact Omni_auth is like 2 gems in one. Since It passes off most all of the burden to verify the input fields sent to other large websites. I do mean verify. Without Omni_auth I would have to write code to verify that correct characters were used. The input is within limits. Not too few or many characters. Its a lot of work done with a little bit of code.
