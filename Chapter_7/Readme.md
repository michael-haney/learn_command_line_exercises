#Chapter 7: Remove Directory (rmdir)

##Do More

###Make 20 more directories and remove them all.

Command used `mkdir -p alpha/bravo/charlie/delta/echo/foxtrot/golf/hotel/india/juliet/kilo/lima/mike/november/oscar/papa/quebec/romeo/sierra/tango`
`cd alpha/bravo/charlie/delta/echo/foxtrot/golf/hotel/india/juliet/kilo/lima/mike/november/oscar/papa/quebec/romeo/sierra/tango`
`cd ..`
`rmdir tango`
`cd ..`
`rmdir sierra`
`cd ..`
`rmdir romeo`
etc..

###Make a single path of directories that is 10 deep and remove them one at a time just like I did above.

Command used `mkdir -p alpha/bravo/charlie/delta/echo/foxtrot/golf/hotel/india/juliet`
`cd alpha/bravo/charlie/delta/echo/foxtrot/golf/hotel/india/juliet`
`cd ..`
`rmdir juliet`
`cd ..`
`rmdir india`
etc..

###Comments

I'm sure there is a command to force delete a directory that has contents in it.

##English Questions

###Can you remove the tmp directory?

Not to my knowledge.
