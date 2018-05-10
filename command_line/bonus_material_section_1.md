## Bonus material for Section 1

Here are some other handy commands--try them out in the terminal and see what happens (I’m using the `>` character to represent the prompt):

```
  > cal
  > cal 1945
  > cal 11 1971
  > date
  > date '+%Y-%m-%d'
```

Using that last date command as an example (and maybe looking at the man page) figure out how to print the date in a format like 6/24/17.

What does the format '+%s' print?  What is this number?  (Read more at https://en.wikipedia.org/wiki/Unix_time)

ASCII and Unicode are two different ways to encode characters.  Most of what you do in the terminal is ASCII.  If you look at the ASCII chart (try `man ascii`) you'll see that each letter, number, and punctuation mark is represented by a number between 0-127.

Try this on the command line:

```
  > echo abcde | od -t dC
```

This probably looks like gibberish now but trust me, we'll get to it.  That long vertical line in the middle is the 'pipe' symbol--it's the character above the backslash on the keyboard.  (There will be more about this in section 3). This command is taking the output of the `echo` command and 'piping' it to the `od` command which prints out the value of *raw bytes* from a file in various formats.  So what you get is the ASCII values of the letters.

It should output something like:

```
  0000000    97  98  99 100 101  10
```

This shows the ASCII value for each letter *a* through *e*.  What does the 10 represent?

The tutorial mentioned the 'archaic long s' character.  This character is represented by Unicode because Unicode can represent 1000's of characters by using multiple bytes (not just 0-127).  So virtually any character or glyph from any language can be encoded with Unicode.
First off, you need to know the Unicode 'code' for this 'archaic long s'.  Go ahead and Google and see if you can find it (hint: may belong in the 'Latin extended-A' section).

Now, there's a lot of variation in how terminals handle Unicode, but this should work in your Ubuntu terminal as one method to print Unicode characters:

```
  > echo -e "\u00a9"
  > echo -e "\u03a8 \u03a9"
```

What are the Unicode characters output by the above commands?
If you’re crafty, you might find a way to output some emoji in the terminal using Unicode.

