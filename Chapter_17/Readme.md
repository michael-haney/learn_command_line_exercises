#Chapter 17: Finding Files (find, DIR -R)

##Do More

###Look for all the video files on your computer starting at the home drive and use the > to save the list to a file. Remember how you can do SOMECOMMAND > SOMEFILE.txt and it will write the output of SOMECOMMAND to the file SOMEFILE.txt?

```
$ pwd 
/Users/Michael/workspace/davinci_coders_t1_2016/homework/learn_command_line_exercises/Chapter_17

$find ~/workspace/davinci_coders_t1_2016/DaVinci_Videos_T1_2016/in_class -name "*.mp4" > Videolist.txt
```
##English Questions

###Can you show me all the files in slash temp slash foo?

```

###What log files are in your log directory?

find log.directory -
