---
layout: page
title: Shell Tools 
permalink: /shelltools/
---
## 0. Table of Contents
1. Background  
* the whats and whys of shells. 

2. Shell Introduction
* shell program 
* zsh vs bash 
* other common shells
* child processes

3. Core Usage

4. Scripting 

5. Real Use Cases 

6. Adavanced Topics

7. Sources and Further Reading


<br/><br/>

## 1. Background  
In this module, we will dive into the world of shell, exposing the many underutilized tools available allowing you to utilize your computer to it's maximum potential. "Computers these days have a variety of interfaces for giving them commands; fanciful graphical user interfaces, voice interfaces, and even AR/VR are everywhere. These are great for 80% of use-cases, but they are often fundamentally restricted in what they allow you to do — you cannot press a button that isn’t there or give a voice command that hasn’t been programmed. To take full advantage of the tools your computer provides, we have to go old-school and drop down to a textual interface: The Shell. Nearly all platforms you can get your hand on has a shell in one form or another, and many of them have several shells for you to choose from. While they may vary in the details, at their core they are all roughly the same: they allow you to run programs, give them input, and inspect their output in a semi-structured way. (1)" Note that is assumed you have some basic knowledge of the shell in these modules.

<br/><br/>

## 2. Shell Introduction 
A `shell program` is (typically) an executable binary whose commands are turned into system calls to the operating system application programming interface, or `OS API` for short. In this module, we will use the `zsh` which is built on `bash`. Feel free to use either: note that `zsh` is more interactive and customizable than `bash`. Learn more about setting up `zsh` [here](https://github.com/ohmyzsh/ohmyzsh/wiki/Installing-ZSH). 

In addtion to `bash` and `zsh` there are other used shells like `sh`, `ash`, `dash`, `ksh`, `tcsh`, and `tclsh`. These shells have different syntax and vary is subtle ways, but since shells are also programs, you can run one inside of another. Lets test this. Open up your terminal and enter the follow, note that `echo $0` displays what shell you are using, and `exit` closes the shell:
```
tcsh
echo $0
exit
echo $0
```
You should see the first `echo $0` outputed `tcsh` and the second outputted your original shell. The `tcsh` process is a child process, meaning it is a process created by another process (the parent process). Try running `sh` and then `echo $0` to solidify your understanding of the basic child-parent idea. We will talk alot more about processes later.

Let's look at some commands that will help you identify your system. Try running:
```
id
```
This will show you a bunch of data about related to user and group names. Now try: 
```
w
```
This will show you who is logged in. You can also get specific with `w hi USERNAME-ON-YOUR-MACHINE` and the shell will show you where a user is logged in from.

There are also many ways to get help. You can use either `man` or `info` to obtain details and usage about certain commands. Try running:
```
man echo
```

## 3. Core Usage 
Before we dive deep into some core commands used in zsh, we first have to understand the special characters recongized by the shell and the differences between single and double quotes. From your working directory (recommending to first create a new folder on your desktop and navigate to it. Use `mkdir` from the desktop directory to make a new directory and navigate to the folder using `cd <pathtofoldername>`), and enter the following commands: 
```
touch file1 file2 
ls *
echo *
```




## 4. Scripting 

## 5. Applicable Use Cases

## 6. Advanced Topics 

## 7. Sources and Further Reading
* An incredible open-source MIT lecture and page about Git and Github. Goes very in depth about Git's data model and inspired alot of this writing. Visit this page [here](https://missing.csail.mit.edu/2020/course-shell/).

* A complete in depth and detailed look at Linux Terminal tools by Ketan M. I highly recommend for advanced readers. Visit this page [here](https://ketancmaheshwari.github.io/pdfs/LPT_LISA.pdf)

