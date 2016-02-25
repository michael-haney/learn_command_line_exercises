#Chapter 10: Copy A File (cp)

##Do More

###Use the cp -r command to copy more directories with files in them.

I copied all of my desktop folders (and their files) into something/

Command used `cp -r ~/desktop something`

###Copy a file to your home directory or desktop.

I just reversed this command to get my something directory onto my desktop.

Command used `cp -r something/ ~/desktop`

###Find these files in your graphical user interface and open them in a text editor.

Using Finder, navigate to your hostname, then Desktop, then something.

##English Questions

###Can you copy the foo.txt file to slash temp?  (Create foo.txt first...)

Yes, I can. However, this copied foo.txt to my root temp directory, not the Chapter_10 tmp directory.

Command used `touch foo.txt` 
`cp foo.txt /tmp`

###Can you copy .bash_profile in your home directory to the current directory?

I found my .bash_profile in my home directory by using `ls -a` inside of my home directory.

To copy it to Chapter_10 directory, I use 

Command used `cp .bash_profile ~/workspace/davinci_coders_t1_2016/homework/learn_command_line_exercises/Chapter_10`
I then run a `ls -a` to see the .bash_profile now here.

##What is Robocopy?

Robocopy is a command line tool used by PC users to copy file data. We use Macs!
