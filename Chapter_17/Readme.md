#Chapter 17: Finding Files (find, DIR -R)

##Do More

###Look for all the video files on your computer starting at the home drive and use the > to save the list to a file. Remember how you can do SOMECOMMAND > SOMEFILE.txt and it will write the output of SOMECOMMAND to the file SOMEFILE.txt?

```
$ pwd 
/Users/Michael/workspace/Davinci_videos_DaVinci_Videos_T1_2016_in_class

$find . -name '*.mp4' - print > /Users/Michael/workspace/DaVinci_Videos_T1_2016/in_class/Videolist.txt
```
##English Questions

###Can you show me all the files in slash temp slash foo?

```
find /tmp/foo -name '*' -print
/tmp/foo
/tmp/foo/ex12.txt
/tmp/foo/production.log
/tmp/foo/Readme
/tmp/foo/some_file.txt
/tmp/foo/test.txt
```

###What log files are in your log directory?

```
$ pwd
/Users/Michael/workspace/davinci_coders_t1_2016/homework/learn_command_line_exercises/chapter_17/log
$ find . -name '*.log' -print
./production.log
./test.log
```

###Run find in the class directory, pipe the output to pbcopy and create a gist with the content. Paste the Gist URL as a comment on this story.
```
$ pwd
/Users/Michael/workspace/davinci_coders_t1_2016/
$ find . -name '*' -print > homework/learn_command_line_exercises/Chapter_17/pbcopy.txt
```

###Gist URL

https://gist.github.com/michael-haney/071d7773a02709c5c901
