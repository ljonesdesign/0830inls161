# Command Line Interface class notes for August 30, 2017

All of these commands can be studied in more depth by reading the Server Session Preparation Materials or links on that page below the Task box.

[What is the Bash Shell?](https://en.wikipedia.org/wiki/Bash_(Unix_shell))

GIT BASH prompt (BASH stands for Born Again SHell)

```
   1        2                   4a
   |        |                    |
   username@computername MINGW64 ~
   $
   |
  5a

 MINGW64 is just the brand of the terminal, ignore it
```

MacTerminal:   
```
   1        2           3 4a 5a
   |        |           |  |  |
a) username@computername:  ~  $  
b) username@computername:  /  #
                           |  |
                          4b 5b
```
```
1 )       User Name
2 )       Computer Name
3 )  :    specific to mac Terminal
4a)  ~    means home (user) directory
4b)  /    means root directory
5a)  $    means normal mode; normal permissions
5b)  #    your are logged in as root; be careful!
```

SYNTAX

How syntax works (Expanded for ease of understanding):
```
command   applys to:   directory
     ||                |    |
     cd                ~/.ssh  

command applys to:  filename    applys to:   new filename
     ||            |        |                  |       |
     mv            index.html                  home.html  careful! This overwrites home.html if it exits.


command applys to: filename applys to:      exist. directory and current or new filename
     ||            |          |                  |                  |
     mv            portrait.jpg                  images/portrait2.jpg  
                               
```
COMMANDS

You will not master these all today! You have time during networks session, basics lab session
and we will work on these during the webs sessions, so you have 9 more classes to get these commands
learned.

```
pwd         # see your present working directory
touch       # create a new file
clear       # clears the screen by moving it up, does not delete
cd filename # change directory
cd dirname  # will autocomplete to the change in file name
up arrow    # cycle through commands
down arrow  # cycle through commands
cd ..       # move up a directory
cd /        # move to the root directory
cd ~        # go to the home directory
cd -        # go to the previous directory we just came from
cd ../..    # move up two directories
cd ~/.ssh   # move into the user directory with a specific subdirectory

ls          # list files and directories
ls -a       # list all files including hidden files
ls -l       # list long format
ls -la      # list all files and in long format
cp one two  # copy
mv          # move and rename
rm          # remove file (delete) NO UNDO FOR THIS!!! won't remove a directory
rm *.jpg    # remove all files ending in .jpg     
rm -r       # remove recursively. Use this to delete directory and contents
mkdir       # make a directory
cat         # see two or more files, or use it to
              just view one file (like our ssh public key)
|           # pipe command; runs more that one command at once

>           # used with the cat command to create one file out of two             
              Example: cat file file2 > file3  
```

EDITORS
```
vi or vim   #  vim command line editor
nano        # nano command line editor
```

GIT
```
Git commands we will cover:

git init                 # create
git add .                # stage
git commit -m "message"  # commit
git push                 # sync up to server
git pull                 # sync down to client
git log                  # see history
git status               # where are you? Created? staged? committed? 

more                     # see the link below
less                     # see the link below
head                     # see the link below
tail                     # see the link below</pre>
```

<p><a href="https://2buntu.com/articles/1491/viewing-text-files-on-linux-cat-head-tail-more-and-less/">Viewing text files on linux - cat, head, tail, more and less</a></p>

<p>This official Git tutorial is very helpful: <a href="https://try.github.io/levels/1/challenges/1">https://try.github.io/levels/1/challenges/1</a></p>

<h2>How to Check if you have Git Installed:</h2>

<pre>
git --version</pre>

<p>Result if installed (you may have a different version):</p>

<pre>
git version 2.10.0</pre>

<p>Result if not installed:</p>

<pre>
-bash: git: command not found</pre>

<h2>Add your User Name&nbsp; to Git:</h2>

<p>(This is not necessarily your github account username, but it can be. you can do first and lastname if you like:</p>


```
git config --global user.name "myfirstusername mylastusername"</pre>
```

<p>(<a href="https://www.youtube.com/watch?v=xKVlZ3wFVKA">Diference between Git and Github; 2 minute youtube video</a>)</p>

<p>Add your email to git:</p>

```
git config --global user.email myemail@live.unc.edu</pre>
```

<h2>List your git config</h2>

<p>Enter the following:</p>

<pre>
git config --list</pre>

<p>Result:</p>

<pre>
user.name=myusername (or last name too, if you set it up that way)
user.email=myemail@live.unc.edu</pre>

<p>Stages</p>

<ul>
	<li>Committed</li>
	<li>Staged</li>
	<li>Modified Stage</li>
</ul>

<p><a href="https://help.github.com/articles/setting-your-username-in-git/">https://help.github.com/articles/setting-your-username-in-git/</a></p>
