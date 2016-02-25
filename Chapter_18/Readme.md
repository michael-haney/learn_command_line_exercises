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
