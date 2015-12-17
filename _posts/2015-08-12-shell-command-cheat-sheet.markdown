---
layout: post
title:  "Commonly Used SSH/Shell Commands (SSH Cheat Sheet)"
date:   2015-08-12 14:18:50
categories: blog
author: "Brad Hopkins"
authorbio: "I bought my first computer - an Apple Performa 6320 - when I was in college and have been building websites ever since. I like long walks in Illustrator and candle lit dinners with ExpressionEngine."
authorphoto: "/images/bio-gbradhopkins.jpg"
---
Here are some of the most commonly used SSH / Shell commands for those that are unfamiliar with using the command line. 

_Honestly, this is a cheatsheet for me. Hopefully someone else will find it valuable._

**How to move into another directory.**

Use command below to change directory
	
`cd [another directory]`

_example: move to directory “download”_
	
`cd download`

**How to go to home directory**
	
`cd ~`

**How go to the last directory you were in**
	
`cd -`

**How to go up a directory level**
	
`cd ..`

**How to show the full path of the current directory**

Use this command to find out where are you currently in.
	
`pwd`

**How to list files and/or directories in a directory**
	
`ls `

_(just type ls and hit enter)_

**How to list all files and information**
	
`ls -al`

**How to list all files ending with certain extension**
	
`ls *.ext`

_example:_
	
`ls *.php`

**How to list all files and folders with detailed information including file size**
	
`ls -alh`

**How to quit and exit SSH client**
	
`exit`
