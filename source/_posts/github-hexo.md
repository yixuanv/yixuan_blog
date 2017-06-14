---
title: Github+Hexo[basics]
date: 2017-06-12 17:36:01
tags:
- Technology
---

Hexo is a very useful tool to build static websites and it has lots of simple and beautiful themes to select. Here are few tips that I conclude: (Mac OSX)


1. create a github account and generate ssh keys. Do not create two accounts at the same time or it will bring trouble!!
2. create a new respository and a new file (`mkdir`) called "blog" and follow its instructions:

	```bash
	git init
	git add .
	git commit
	```

3. install `node` and xcode
4. install hexo in "blog" file: sudo npm install -g hexo
5. Setup

	```bash
	hexo init
   hexo generate
   hexo server
   ```
6. create a new respository called your_user_name.github.io
7. revise _config.yml file to:

   ```yaml
   deploy:
     type: git
     repo: https://github.com/username/username.github.io.git
     branch: master
   ```
8. npm install hexo-deployer-git --save
9. hexo generate
10. hexo server 
10. hexo deploy

## what should I do if create two accounts?

In the settings, we can transfer the respository into another account then delete one account.

## Done!
![](http://blog.zhangruipeng.me/hexo-theme-hueman/gallery/math.jpg)

