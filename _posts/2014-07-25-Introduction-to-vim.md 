---
layout: post
title: Introduction to Vim
location: Bhubaneswar
tags:
- vim
---
<br/>
Well if you are new to vim or linux or a wannabe programmer this post is surely for you.As you google about vim you will get hell of a lot of answers which gets complicated as the more you read them.So only read the wiki artilce to get the story.And the moment you start using it you will realise it's not your cup of tea and can't be learnt in a day.<br/><br/>


First thing first ,if you are using windows then don't try to install vim on it cuz it's more than a Install and a I agree box.It will get way more tougher than you think.<br/>
Vim is a primarily a terminal based application.
Vim works best on linux and unix based systems.<br/>
Well I meant you must use ubuntu or apple.Fedora will work fine too.<br/>

So go to your terminal and type:
<pre>sudo apt-get install vim</pre>  
<br/>

<code>apt-get</code> is for ubuntu  
replace it with <code>yum</code> if you are using fedora.

So let me explain you the file structure of vim:<br/>


First of all, after installing you have to manually create a folder called .vim and a file called .vimrc on the Home directory of your machine. <br/>

<pre>

.	Home
	├── .vim(folder)
	│   └── I keep all the subfolders and important files.
	│   
	└── .vimrc(file)
		└── I am thes monster you must understand before using vim
	    
</pre>

<code>These are dotfiles begins with dots so are hidden in linux.To see them type "Ctrl-h". </code><br/>

Both the .vimrc file and the .vim folder are used to configure vim editor.Initially you will get a version of vim which will nothing cooler than a terminal:P.
In this blog I will talk about .vimrc .<br/>

Well vim is a very powerful text editor.So to maintain it or configure it uses a Language called VimL and can use other scripting languages too.<br/>
So,copy the following and paste it on your <code>.vimrc</code>.
<pre>
set number
colorscheme darkblue
abbr teh the
abbr email <your_email@gamil.com>
</pre>

Now open up your vim editor.

You will see the number lines in vim and backgruound changed.And type "teh" a common spelling mistake.You will see them automaticaly get corrected.<br/>

If you don't see them.Then probably vim may not opening .vimrc at startup and you need to manually configure it.
TO check hit  <ESC> :scriptnames.
See if there is a vimrc is mentioned.If not google about how can you configure vim startups to point to .vimrc.You will probably find a lot of commands and solution online.
<br/>
If there is no problem.
Then lets get started with vimrc.
Vim works in three mode insert ,visual and normal.

You can map any command  to the keystrokes in the three modes:
<pre>
imap,vmap&nmap 

and 
combo mapping like nnoremap,inoremap and bunch of others.

</pre>

This shows you the [list](http://vim.wikia.com/wiki/Displaying_the_current_Vim_environment) of all the mappings.

A very important thing ,the commands you type in the vim panel are the same thing you can write in your vimrc file.

Actually the only thing vim does is runs the file vimrc at the startup.
Hence you see the command above in vimrc can be written through your vim terminal hitting escape like:

:colorscheme blue
:set number

Lets change a few more things in .vimrc and restart vim.

<pre>
nnoremap &lt;C-h&gt; :tabprevious&lt;CR&gt;
nnoremap &lt;C-l&gt;   :tabnext&lt;CR&gt;
nnoremap &lt;C-t&gt;     :tabnew&lt;CR&gt;
</pre>

In your vim terminal
hit ESC  and write <code>:tabnew</code> 

Now in vim hit <code>ctrl-t , ctrl-h , ctrl-l</code>.
<br/>
So lets see other peoples <a href="http://www.dotfiles.org/.vimrc">vimrc</a>.
<br/>
Now lets source a vim file.Copy this fila <a href="http://www.dotfiles.org/~omab/.vimrc">vimrc</a> to your <code>.vim</code>name it <code>test.vim</code>.<br/>

go to your vimrc:
and add:

<pre>

"source files
source ~/.vim/test.vim

The structure:

.	Home
	├── .vim(folder)
	│   ├── test.vim
	│   └── other files and folders you don't need to bother.
	└── .vimrc(file)
		└──
</pre>

<h3>Hacks you should try</h3><hr>
Check your new vim .Try other configuration too but don't source them all together.