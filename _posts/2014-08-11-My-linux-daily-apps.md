---
layout: post
title: My linux daily apps
location: Bhubaneswar
tags:
- linux
- dotfiles
---

How do you maintain your projects with all the devices and application in a perfect sync?How do you work perfectly in a order that effectively makes your work smoother and effective.Well the answer could be *dropbox* but still I am talking about a more synchronized way of doing things on your linux machine. 







>What do you call your zen of workflow?

##How should I do things then?

Well I was taking about a few apps and settings that can boost your productivity in daily life.
But these are mostly ncurses apps and are seriously good...
Before you use them...few things you need to learn.





<!--excerpt-->



##Learn to confgure your linux

>Linux is kind of like a piece of open art.It only 
gets beautiful for you the way you paint(configure) it.

I am not talking about the gui tools and application.Without further ado...

So here's the list:

* tmux
* youtube-dl 
* cmus 
* mplayer 
* pyradio 

These are some of the ncurses that you can use for daily use can.And trust me they will provide more functionlity then anything you have ever seen.I will look like these...	
![advanced_terminal_photo](/assets/2_1.png)


###Advantages:

* mplayer lets you play music through terminal.
* cmus is a ncurses music player
* youtube-dl as name suggests 
* tmux is the terminal multiplexer (it lets you create sessions and divides terminal to small screens as shown) 

Installation 

```
sudo apt-get install tmux
sudo apt-get install youtube-dl
sudo apt-get install cmus
sudo apt-get install mplayer

```




##youtube-dl hacks

You can use it to not only get videos but music also.

You can use it to download music from soundcloud and myspace.Well the proper word will be called stream.Let me show how!!


Right click on your song and copy link location and attach the url at the end of youtube-dl on your terminal.

![youtube...soundcloud](/assets/2_2.png)  

![youtube...terminal](/assets/2_3.png)  

![youtube...myspace](/assets/2_4.png)  

You can also do this on myspace.Cool ,no IDM shit any more...just copy and paste this sucker.


##Cmus

Cmus is one of the best ncurses music player you can have.
It comes with tons of functionality ranging from creating playlist,listed names by artist to creating queue and a lot more.

Just hit 1 2 ... and all the numericals and you will see all the music.But initially you will need to add a directory from where it reads the listed songs for keeping it local and stuffs.

Just to help with to add all the music in a folder you just need the following command:
hit ```ctrl-C ``` then  ```:add ~/Music```.

```
Hit enter to play 
Hit c to stop
Hit e to add to queue
```

>This [tutorial](https://github.com/cmus/cmus/blob/master/Doc/cmus-tutorial.txt) will give you enough experience.

>Want to know [more about cmus](http://www.tuxarena.com/static/cmus_guide.php) about cmus?
	

And yes _ cmus won't work without mplayer_.So don't forget to install mplayer.



##Tmux 


Tmux is a monster like vim.It's keystrokes and mappings are kind of tough for beginners.I will soon give my openion about it and most importantly dotfiles.Dotfiles are the way you customize your whole system.Figuring out your dotfiles will definitely make you a good programmer and enhance your skills.Hang on for next few posts to know more about tmux.
