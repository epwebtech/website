---
layout: post
title:  "Publishing a Jekyll Site on  Gituhub"
date:   2015-08-18 18:18:50
author: "Brad Hopkins"
authorbio: "I bought my first computer - an Apple Performa 6320 - when I was in college and have been building websites ever since. I like long walks in Illustrator and candle lit dinners with ExpressionEngine."
authorphoto: "/images/bio-gbradhopkins.jpg"
categories: blog
---

To publish your site on Github pages, use the following steps in the terminal and / or Github.

1. In the terminal, switch to the directory that you want to publish to Github. `cd {directory}`
2. Initialize the directory. `git init`
3. Shows the status of the files in the directory. Red indicates not committed. Green indicates committed. `git status`
4. Start tracking the files with Git. `git add .`
5. Commit the files and provide a commit message. `git commit -m 'Initial Commit Message'`
6. Create a new repository in your Github account.
7. Push the local repository to your Github account using the commands provided under the "_…or push an existing repository from the command line_" section. 
- `git remote add origin https://github.com/username/repositoryname.git`
- `git push -u origin master`
8. Create a local branch for the project pages site. It **MUST** be named gh-pages or it will not display as a website. `git checkout -b gh-pages`
9. Push the new branch to the remote repository. This command not only pushes the files to Github but also creates the new branch. `git push origin gh-pages`

Once the gh-pages branch is pushed, it will take no more than 10 minutes for the site to be available.

Github project pages are located at the following domain: username.github.io/repositoryname

##Where'd my styles go?

Github pages are hosted from a sub-path, so we need to set a base URL configuration in our project.

1. Edit the `_config.yml` file baseurl variable by adding the name of the repository with a leading slash `/repositoryname`
2. Commit the files and push to the `gh-pages` repository

##Removing a local Git repository

The command `rm -r .git` removes the local Git repository for a project.
