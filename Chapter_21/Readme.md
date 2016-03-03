#Chapter 21: What's In Your Environment (env, echo, Env:)

##Do More

###I want you to go online and research how you change your PATH for your computer. Try to do it entirely from the CLI.

Lets first look at our path.
```
$ echo $PATH
/Users/Michael/.rvm/gems/ruby-2.2.4/bin:/Users/Michael/.rvm/gems/ruby-2.2.4@global/bin:/Users/Michael/.rvm/rubies/ruby-2.2.4/bin:/usr/local/bin:/usr/bin:/bin:/usr/sbin:/sbin:/Users/Michael/.rvm/bin
```
You can add onto the path by setting the `PATH` equal to your current path + whatever you'd like to add onto it. For instance
```
$ PATH=/Users/Michael/.rvm/gems/ruby-2.2.4/bin:/Users/Michael/.rvm/gems/ruby-2.2.4@global/bin:/Users/Michael/.rvm/rubies/ruby-2.2.4/bin:/usr/local/bin:/usr/bin:/bin:/usr/sbin:/sbin:/Users/Michael/.rvm/bin:usr/sbin
```
This only temporarily updates your path, once you exit Terminal and reopen, that path will no longer exist.
To add a path permanently, we need to create a .bash_profile file in your home directory and set the path there, then save it.
```
$ export PATH="example/path:$PATH"
```

##English Questions

###What is your shell set to?

To figure this out I will use the command `env` and grep my SHELL.
```
$ env | grep SHELL
SHELL=/bin/bash
```
I see here that my shell is set to bin/bash

###What directory are you in (don't use pwd this time)?

Similar to the method I used in finding my shell, I will use to find my pwd.
```
$ env | grep PWD
OLDPWD=/Users/Michael/workspace/davinci_coders_t1_2016/homework/learn_command_line_exercises
PWD=/Users/Michael/workspace/davinci_coders_t1_2016/homework/learn_command_line_exercises/Chapter_21
```
This is useful for showing the last directory I was in as well. However, you can also just use
```
$ echo $PWD
```

###What is your home directory set to?
This time I will use $ to designate the environment I am searching for, similiar to the one listed above that was included in the reading.
```
$ echo $HOME
/Users/Michael
```

###Can you set your environment to have DEBUG set to true?
I can. First however, I noticed that there is no DEBUG environment. Using 
```
$ echo $DEBUG
```
and
```
$ env | grep DEBUG
```
both return nothing. From here, I export the variable DEBUG and set it to true.
```
$ export DEBUG='True'
$ echo $DEBUG
True
```
