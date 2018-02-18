# CSESoc Getting Started Guide  

## Hi there. 😀

![hello adventurer](https://i.imgur.com/Hrw8bfI.jpg)

Hello adventurer, welcome to CSESoc's Getting Started Guide<sup>TM</sup>. Here we walkthrough using the CSE lab computers, and also what you need to get started from home. Visit one the CSE labs (found here  http://taggi.cse.unsw.edu.au/FAQ/CSE_lab_map/) or if you aren't on campus just sit tight and follow along!

You might be itching to get started, or you might be uncertain of what to expect, never fear! The GSG<sup>TM</sup> is here to answer your questions and calm your restless souls.

Along this first quest, and throughout the semester you will at times get bogged down and stuck, that's okay! You are not in this alone. Seek help from your fellow adventurers, or from a friendly and wise sage (your tutor!).

Ok, so today we are taking it from the top. The aim is to get you familiar with the CSE Lab computers, and the basics of this thing called *Linux*.


## Why should I learn this *Linux* thing? 🤨

Oh! I'm glad you asked. You may be thinking, I have my own computer or laptop. Maybe it's running a Windows or macOS [operating system](https://www.slideshare.net/11southongeorgeb/the-purpose-of-an-operating-system). That's totally fine, both of these work great for programming. But for true hacker street cred, you'll want to at least know the basics of Linux. Oh, plus you have to use the CSE computers to do your **exams** and submit **assignments**, important stuff!

![Hacker meme](https://i.imgur.com/Qaqey7c.jpg)


## Can we get started already? 🤓

Alright alright, let's jump right in. Your first task is to log in. 
1. Type your zID (eg. z5555555), then press enter
2. Type you zPass, then press enter

By logging in you agree to the UNSW ICT policy, be sure to use the computers responsibly. https://www.gs.unsw.edu.au/policy/documents/ictpolicy.pdf 

Once you are in, you should see a desktop and a menubar. Feel free to check it out and see what's on there. You can right click on the desktop to see some more delicious menus.

![screenshot](https://i.imgur.com/kTTFLRu.png)


## Too easy. 💪

Hey, we are just getting started here. Next task is to open this guide. Open Firefox by going `Applications Menu` -> `Internet` -> `Firefox ESR`

The URL is [URL]
# FIXME - add the url!

![screenshot Firefox](https://i.imgur.com/HrSifZG.png)

The next place you want to visit is your course page. You can find it quickly just by googling "comp1511 18s1", which is the course code and the session (20**18** **s**emester **1**).

It should be the top hit, but if you can't find it I have the url for you right here:
https://webcms3.cse.unsw.edu.au/COMP1511/18s1/ 

![screenshot webcms](https://i.imgur.com/4uCcnJ6.png)

> ℹ️ Just change the url if you are in COMP1911 or (postgrad) COMP9021

Login with your zID and zPass again, and then get familiar with what's on there. You can always come back and read more of it later.


## How am I going to stay up to date with all this? 😦

Course notices and comment threads you are subscribed to will go to your email. Your email address will look something like z5555555@student.unsw.edu.au, but with your own zID.  

For email, there are 3 options:

1. Use webmail in a browser: https://outlook.office365.com
    - Username: zID@ad.unsw.edu.au
    - Password: zPass
    - Notice the username has @ad, not sure what that stands for `¯\_(ツ)_/¯`,  
    it's just used for your username.

2. Use a mail client on your own computer and/or phone
    - Check out section 2.2 or section 2.3 here: http://taggi.cse.unsw.edu.au/FAQ/Office_365_Email/

3. Redirect your mail to your own email account (like your gmail)
    - You can redirect your mail with the UNSW Identity Manager here: https://idm.unsw.edu.au
    - You will probably also want to be able to send emails, not just receive them. Here is a guide on how to set up a gmail alias: https://support.google.com/mail/answer/22370 



## Is it time to start coding? 🙃

Patience young padawan, first you must learn the power of the terminal.

![star wars meme](https://media.giphy.com/media/R1o1UUf1hSRBS/giphy.gif)

First up, open a terminal by right clicking on the desktop and choosing "Terminal" (you can also find it in the menus).

![screenshot terminal](https://i.imgur.com/Bvq5I5B.png)


## What is all this cryptic symbol stuff? 🧐

The stuff that appears before the cursor is called a prompt. That just means that you can type and enter terminal commands.  
Let's try out our first command. 

Type 
```
echo "Quack!"
```
and press enter.

It prints out "Quack!", just like an echo right? Except in real life duck quacks don't echo (true fact!).  
Ok ok, let's try something a bit more interesting.

Type 
```
pwd
```
 and press enter. 

Another name for folders is directories, and `pwd` is short for "**P**rint **W**orking **D**irectory", ie. print out the directory we are currently in. Since we just opened the terminal, we will be in the "home" directory. This is were we start when we open a new terminal.

> ℹ️ Oh, so this is cool; any files or directories you put in your home folder can be accessed on any lab computer, just by logging in.


## `echo` and `pwd`, ok I'm ready for more commands! ✍️

Ok then, these next ones will be some of your most used commands.
Try entering this command: 
```
ls
```
`ls` is short for list, and it will list the files and sub-directories in the current directory.

Here's another:
```
cd
```
 -- "**c**hange **d**irectory". It's like opening a folder!

We have to tell the cd command which directory we want to change into however, so you can try 
```
cd Desktop
```
To go back up to the *parent* directory, we can use 
```
cd ..
``` 
Have a try!

> ️ℹ️ To get back to the home folder you can use `cd ~`. The `~` (tilde) symbol represents your home directory.


## Can I make new directories? 🤔

Sure can, the command is `mkdir`. Let's make a folder where you can store your coursework.

Type 
```
mkdir COMP1511
```

Now if you try `ls`, you should see that there is a new directory called "COMP1511".

Now let's change into this directory, you remember how! You can use `pwd` to check that you were successful.


## Phew, that's a bunch of things to remember. 😰

True, but you will be `cd`-ing and `ls`-ing so much that it will be muscle memory in no time. Let's summarise:

| Command       | Description
| ------------- |-------------|
| `echo`        | echo back some text |
| `pwd`         | show the current working directory  |
| `ls`          | list files in the current directory  |
| `cd`          | change directory      |
| `mkdir`       | make a new directory      |

Here are a few terminal tips that will save you a tonne of time:

### Reuse previous commands
Hitting the "up" key will automatically place a previously executed command at the prompt. Going down, of course, does the opposite if you need it

### Tab Completion
Essentially completes a filepath you have half-typed out so you don't have to waste precious milliseconds writing the rest of it. It is magical.

You can try this out with the `cd` command. Make a folder with a really long name and then tab-complete the name when you cd into it. An example might be:

```sh
mkdir antidisestablishmentarianism
cd anti<tab> <enter>
```

Try it, your life is now measurably better.

![I know kungfu](https://i.imgur.com/uBW5gqv.jpg)

### Pasting in the terminal
Copy and past might work a bit differently from what you expect. Usually `Ctrl-c` is copy and `Ctrl-v` is paste. This will work in Firefox, but in terminal these keys have special meanings. `Ctrl-c` is used to abort the current program, and `Ctrl-v` is for inserting special characters. So how can you copy and paste then?
all you have to do is 
1. select the text you want to copy, 
2. switch to your terminal (you can use `Alt-Tab`) and then, 
3. click the middle mouse button (press down on the scroll wheel).

You may also be able to right click in the terminal and choose paste, or use `Ctrl-Shift-v`.


## Alright, I'll try to remember those tips. What's next? 😅

Now we get to the programming. To write programs we use a text editor. Here is a breakdown of your options on the CSE lab computers:
- `gedit` - a graphical editor.
- `nano` - a basic editor that you can use a terminal.
- `emacs` - an advanced editor with many, many shortcut keys, can be used in a terminal.
- `vim` - another advanced editor, and it's the best one (I'm not biased at all!). It takes a while to learn. Works in a terminal.

For now we will start out with the easiest one, `gedit`. If you are feeling super confident and want to learn one of the advanced ones, come back and check out these links later:
- Vim guide: https://hackmd.io/s/HyVewBVW 
- Emacs guide: https://jashankj.space/emacs.pdf  

Also keep an eye out for CSESoc's Vim and Emacs workshops!


## Ok, how do we get started with Gedit? 😋

First, `cd` into your `COMP1511` directory, and then type:
```sh
gedit hello.c &
```
This will open the Gedit text editor in new window with a new file, "hello.c". The ampersand allows us to keep using the terminal while Gedit is open.
Since this is probably the first time you have used Gedit, we want to set up some of the options. Here are the recommended settings:

![screenshot Gedit settings 1](https://i.imgur.com/3sI7mEd.png)
![screenshot Gedit settings 2](https://i.imgur.com/Fq8qEEA.png)

> ℹ️ If you are coming along for the ride but you aren't at a CSE lab computer right now, you can follow along here: https://repl.it/languages/c (just click run to *compile*).

Now we can start to code! Our aim is to create a simple C program that can print out "hello world!". Type this code out into Gedit. It's okay if you don't understand it just yet.

![screenshot hello.c](https://i.imgur.com/SoH4xUB.png)

Be careful to get all the symbols and spacing correct. For line 7, you can get 4 spaces at the start of the line by pressing `<Tab>`. Line 7 and line 9 have semicolons (`;`) at the end.


## Yo, what did I just write?? 😵

A rough explanation of the code goes something like this:
- Every program we write has a *main* function that looks like this on line 5.
- Inside the main function (between the `{` curly brackets `}`) we put our code.
- `printf` comes from the `stdio.h` file that we included at the top. It prints out some formatted text.
- Then on line 9 we finish the program and let the Operating System know that everything turned out successfully. All according to plan! `EXIT_SUCCESS` comes from the `stdlib.h` file that we included.

![dog at computer](https://i.imgur.com/bSJgxsD.png)

Again, don't worry! You will go over this again in more detail in your lectures, this is just to get your feet wet. You might be wondering what the `\n` is on line 7, that's a "newline character", which will just insert a new line when outputting to the terminal.


## How do we run it? 🤪

Well first we have to compile our code. **Save** the file and switch back to the terminal from before. If you list the files in the current directory now with `ls`, you should see our new file `hello.c`.
Now we can use the `gcc` command to *compile* our code into a program that the computer can understand. 
Try typing out this command, and double check it is the same before hitting enter:
```sh
gcc -Wall -Werror -o hello hello.c
```
That is a lowercase letter o by the way. If there is no output, then that means it worked. If it prints some errors, go back to Gedit and check that everything is the same as the picture.

Now if you run `ls` again, there should be a new item called "hello". Just remember, our code is the file that ends in `.c`, and our program is whatever we put after the `-o` in our compile command.

Now that it is all compiled, let's run our program. Just type:
```
./hello
```
That is, a dot and then a slash and then the name of our program.

![hello world](https://i.imgur.com/0FB6LAi.png)


## It prints "hello world!", it works! 🤩

Yup! You have written your first program. Feel free to experiment with the code and change the message, just remember if you change the code, you will have to compile it again before running it.


## Can I do this on my own computer too? 😮

Yes you can! There are a few different ways to do this.
- Remotely connect to the CSE servers using SSH via the internet
- Write and compile on macOS, Windows
- Install Linux on your computer

There are guides on how to do that here:  
http://www.cse.unsw.edu.au/~cs1511/17s2/home-computing/  

And if you prefer video screencasts, there is a whole playlist right here:  
https://goo.gl/fMa31p 


## Is that the end of our quest? Mission accomplished? 😟

That's pretty much it. I'll just leave you with a couple of tips.
You will be using these three snippets for every program you write, so I recommend just wrote learning them. Spend a short amount of time getting faster at typing them out, and then when it comes to writing more programs you will know how to get started quickly.  
```c
#include <stdio.h>
#include <stdlib.h>
```

```c
int main(int argc, char *argv[]) {
```

```sh
gcc -Wall -Werror -o hello hello.c
```

If you are hungry for more, here are some extra resources:
- CSE Taggi FAQ: http://taggi.cse.unsw.edu.au/FAQ/   
- UNIXverse: http://www.cse.unsw.edu.au/~nicolag/unix/  

Useful for later on in semester:
- Debugging: https://goo.gl/g7MzjL 
- Videos on COMP1511 topics: https://goo.gl/cMWCK2 
- Coding style guide: https://www.cse.unsw.edu.au/~cs2521/18x1/StyleGuide.html 

Okay, that's it, good luck out there adventurer!


## Wait, but… I'll miss you! 😭

No you won't, CSESoc has weekly BBQs, exciting workshops and amazing events planned for throughout the semester! The easiest place to keep up to date and not miss out is the CSESoc Facebook group here:  
https://www.facebook.com/groups/csesoc/ 

> ℹ️ If you are not on Facebook, look out for our weekly email newsletters.

We'll see you again soon! 👋
