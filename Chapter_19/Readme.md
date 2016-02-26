#Chapter 19: Getting Command Help (man, HELP)

##Do More

###Use man or help to look at every one of the commands you have in your list to memorize.

``` 
$ man pwd
```
pwd tells us the path for the current working directory.
```
$ man hostname
```
hostname tells us the name of our current host system.
```
$ man mkdir
```
mkdir will make a directory titled with whatever we specify after.
```
$ man cd 
```
cd will change the directory to whatever whatever directory/path we specify after.
```
$ man ls
```
ls lists every file in the pwd. We can list hidden files with `ls -a` and we can specify what ls will look for. For example, `ls "name of directory"`
```
$ man rmdir
```
rmdir will remove whatever directory we specify after.
```
$ man pushd
```
pushd's manual takes us to a BSD General Commands menu
```
$ man popd
```
popd's manual takes us to a BSD General Commands menu
```
$ man cp
```
cp copies whatever file we specify.
```
$ man mv
```
mv will rename a file or move its location depending on what we specify.
```
$ man less
```
less prints out the content of a file with the functionality of being able to skip forwards or backwards through it.
```
$ man cat
```
cat prints out the file
```
$ man xargs
```
xargs reads space, tab, newline and end-of-line strings.
```
$ man find
```
find will find whatever is specified in a directory and/or file. From here, you can do more to the things you found.
```
$ man grep
```
grep will search for specific keywords/phrases.
```
$man man
```
man shows us the operations behind the command `man` and how we can more specifically search for manuals.
```
$ man apropos
```
apropos searches the what is database for strings
```
$ man env
```
env takes us to the General Commands manual
```
$ man echo
```
echo adds text to a new file, thus creating it, or to an existing file.
```
$ man export
```
export takes us to the General Commands manual
```
$ man exit
```
exit exits a terminal session
```
$ man sudo
```
sudo executes a command as another user
```
$ man chmod
```
chmod changes file modes or access control lists
```
$ man chown
```
chown will change ownership of whatever is specified.

##English Questions

###What option to ls tells it to output file size in human readable form?
```
man ls -@ 
```

###Is there a case insensitive option to grep?
```
man grep
```
-i will ignore the case sensitivity that the grep command alone will output.

###What does the -r and -f options to rm do exactly?
```
man rm
```
-r will attempt to delete all subdirectories inside of the directory in question. -f forcibly deletes the file in question ignoring access rights and even -i.
```
-R       Attempt to remove the file hierarchy rooted in each file
           argument.  The -R option implies the -d option.  If the -i
           option is specified, the user is prompted for confirmation
           before each directory's contents are processed (as well as
           before the attempt is made to remove the directory).  If the
           user does not respond affirmatively, the file hierarchy
           rooted in that directory is skipped.

-r        Equivalent to -R.
```
```
-f        Attempt to remove the files without prompting for confirma-
           tion, regardless of the file's permissions.  If the file does
           not exist, do not display a diagnostic message or modify the
           exit status to reflect an error.  The -f option overrides any
           previous -i options.
```
###What does the ifconfig command do?
```
man ifconfig
```
ifconfig configures network interface parameters.
