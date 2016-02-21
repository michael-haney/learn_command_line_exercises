#Chapter 12: View A File (less, MORE)

##Do More

###Open your text file again and repeatedly copy-paste the text so that it's about 50-100 lines long.

Command used `cd Chapter_12/practice` `touch ex12.txt` `cd ../..` `mine .`
In RubyMine, I type HelloWorld then repeatedly hit cmnd-d to replicate a bunch of these lines.

###Copy it to your temp directory again so you can look at it.

Command used `cp ex12.txt ~/desktop/practice/tmp`
Let's look at it. `less ex12.txt` We use q to quit. `more ex12.txt` Again, q to quit. Spacebar and w to scroll.

##English Questions

###Can we see what's in our production log?

Yes, we can. `less /tmp/production.log`

###What does our database.yml look like?

When viewing it from less, we are prompted to an editor. However, when we do more, nothing happens.
