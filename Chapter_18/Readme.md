#Chapter 18: Looking Inside Files (grep, select-string)

##Do More

###Use quotes to find "new file" and "old file" and "This is".

```
$ grep "new file" *.txt
newfile.txt:This is a new file

$ grep "old file" *.txt
oldfile.txt:This is an old file

$grep "This is" *.txt
newfile.txt:This is a new file
oldfile.txt:This is an old file
```
By using quotes, we are searching for whatever is inside the quotes that also exist in all files that end in .txt 

###Take the list of videos you created (or any other list) and use it to find some videos you want to find.

```
grep "building" *.mp4
```
###Unix: You can use -i to ignore case with grep. Try grep -i new *.txt
```
$ grep -i new *.txt
newfile.txt:This is a new file
```
Similarly, we can ignore all caps.
```
$ grep -i NEW *.txt
newfile.txt:This is a new file
```

##English Questions

###Show me the lines in foo.txt that have "ERROR" in them.
First, I had to add some text in foo.txt with a line that had ERROR in it. I did this on line 3.
```
$ grep "ERROR" *.txt
foo.txt:Line ERROR
```
This method however, did'nt show what line ERROR appeared in. We will need to add `-n` to the command to see.
```
$ grep "ERROR" *.txt -n
foo.txt:3:Line ERROR
```
###Show me the lines in bar.txt that have "davinci" in them.
Again, I had to add a couple lines into bar.txt to include davinci. I also added DAVINCI into oldfile.txt to experiment with.
```
$ grep -i "davinci" *.txt -n
ar.txt:2:davinci
oldfile.txt:6:DAVINCI
```
###Can you print all the lines in text files that have your first and last name in them?
Again, I decided to do some experimenting to see if any of the txt files would return results if they just included my first or last name. I added my first name to bar.txt, my last name to foo.txt and my full name to newfile.txt.
```
$ grep -i "Michael Haney" *.txt -n
newfile.txt:6:Michael Haney
```
It appears, that even though case was ignored, only the exact phrase I searched for was listed. As in the space between my first and last name did not search for two different entities.
