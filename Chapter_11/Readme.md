#Chapter 11: Moving A File (mv)

##Do More

###Move a file in the newplace directory to another directory then move it back.

Command used `pwd` /deskstop/practice/newplace
`ls` oldplace (directory) awesome.txt kinda.txt not.txt
`mv awesome.txt oldplace`
`ls` oldplace (directory) kinda.txt not.txt
`ls oldplace` awesome.txt
Through these steps, we see how and where the awesome.txt file moved.
Now, lets move it back!
`cd oldplace`
`mv awesome.txt ~/desktop/practice/newplace`
`cd ..`
`ls`
oldplace (directory) awesome.txt kinda.txt not.txt

##English Questions

###Can you rename foo.txt to blah.txt?

Yes, I can. 

Command used `mv foo.txt blah.txt`

###Can you move the production.log file in the log directory to slash temp?

Yes, I can.

First we cd into the log subdirectory in the Chapter_11 directory.
Command used `cd Chapter_11/log` 
Next, we make sure production.log is in this directory.
`ls` production.log
It is, so we `mv production.log /tmp` 
We can now check to see it's there.
`ls /tmp`
