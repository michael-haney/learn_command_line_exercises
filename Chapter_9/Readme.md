#Chapter 9: Making Empty Files (Touch, New-Item)

##Do More

###Unix: Make a directory, change to it, and then make a file in it. Then change one level up and run the rmdir command in this directory. You should get an error. Try to understand why you got this error.

Command Used `cd`

Make a directory `mkdir empty`

Change to it `cd ~/empty`

Make a file in it `touch alpha`

Change one file up `cd ..`

Run the rmdir command `rmdir`

rmdir [-p] directory ...

I believe I am getting this feedback telling me to remove the parent directory.

##English Questions

###Can you touch blah.txt?

Yes, I can.

`touch blah.txt`
   
###Let's create foo.txt.

`touch foo.txt`
