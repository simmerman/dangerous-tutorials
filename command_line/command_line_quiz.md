## Command Line Quiz

1. What will be the difference in the output of the following two commands?

```
  > echo  one     two     three
  > echo 'one     two     three'
```

Suppose you had two files as follows:

```
  > cat file1.txt
  This is file1
  > cat file2.txt
  This is file2
```

2. Now you perform the following three commands in order.  What would be the output after each?

```
  > cat file*.txt

  > cat file*.txt >> file1.txt

  > cat file1.txt
```

For questions 3-11, suppose you are in a directory with the following listing:

```
  > ls -laF
  drwxr-xr-x  14 scott  staff      476 Jul  1 11:51 ./
  drwxr-xr-x  50 scott  staff     1700 Jul  1 11:49 ../
  -rw-r--r--   1 scott  staff  3395072 Jun 20 19:52 files.tar
  drwxr-xr-x  13 scott  staff      442 Jul  1 12:18 command_line/
  -rw-r--r--   1 scott  staff     2939 May 25 20:37 notes.txt
  -rw-r--r--   1 scott  staff     3366 Jun 28 20:08 questions.txt
```

3. What's the largest file?
4. Which file has most recently been modified?
5. What subdirectories are in this directory?
6. What user owns the files in this directory?
7. What command would show the files contained in the `command_line` directory?
8. Using `cat` and `wc`, how would you get the total number of lines in all `.txt` files?
9. What command would list all lines (with line numbers) containing the word bash in `questions.txt`?
10. How would you find the file that had the word *mogrify* in its first line?
11. Write one command that moves `notes.txt` and `questions.txt` into the `command_line` directory.

12. How do you create an empty file called `foo`?
13. What are two ways to determine if a file called `zelda.png` is really a PNG file?
14. Why is `rm -rf` dangerous?
15. Let's say you had a `ping` command running in your terminal.  What are two ways to stop it?

For questions 16-21, suppose you had the following directory structure:

```
  /
  |-- etc/
  |-- bin/
  |   |-- wc
  |   `-- cat
  `-- home/
      |-- scott/
      |   `-- answers/
      |       `-- exercise1.txt
      `-- foo/
          |-- hacking/
          |   |-- .vimrc
          |   |-- exploit1.txt
          |   `-- exploit2.txt
          `-- music/
              `-- zelda_theme.mp3
```

From this you can tell that:
  - the root directory is `/`
  - the root directory contains the subdirectories `etc`, `bin`, and `home`
  - the directory `/bin` contains two files, `wc` and `cat`
  etc.

Let's say you're in the `hacking` directory, such that `pwd` shows:

```
  > pwd
  /home/foo/hacking
```

16. From there, what would be the results of the following commands:

```
  > ls
  
  > ls ..
```
  
17. Also from `/home/foo/hacking`, write 2 different ways you could change to the directory containing `exercise1.txt`

18. Write the full absolute path of `zelda_theme.mp3`
19. What's the absolute path of scott's home directory?
20. If you were user scott and you were in `/home/foo/music` and you did `cd`, then where would you be?
21. How could you delete everything within `/home` ?

