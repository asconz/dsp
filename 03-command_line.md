# Learn command line

Please follow and complete the free online [Command Line Crash Course
tutorial](https://web.archive.org/web/20160708171659/http://cli.learncodethehardway.org/book/) or [Codecademy's Learn the Command Line](https://www.codecademy.com/learn/learn-the-command-line). These are helpful tutorials. Each "chapter" focuses on a command. Type the commands you see in the _Do This_ section, and read the _You Learned This_ section. Move on to the next chapter. You should be able to go through these in a couple of hours.

---

### Q1.  Cheat Sheet of Commands  

Here's a list of items with which you should be familiar:  
* show current working directory path
* creating a directory
* deleting a directory
* creating a file using `touch` command
* deleting a file
* renaming a file
* listing hidden files
* copying a file from one directory to another

Make a cheat sheet for yourself: a list of at least **ten** commands and what they do.  (Use the 8 items above and add a couple of your own.)  

Action | Command
------------ | -------------
show current working directory path | `pwd`
create a directory | `mkdir` [options] "folder name"
delete an empty directory | `rmdir` [options] "empty folder name"
delete files and directories recursively | `rm -rf` "outermost folder name"
create a file using `touch` command | `touch` filename.txt
delete a file | `rm` [options] "filename"
rename a file | `mv` orange.txt pineapple.txt
list hidden files | `ls -a`
copy a file to another directory | `cp` [options] SourceFile Destination
display a file's contents | `cat` filename
list existing aliases | `alias`
create an alias | `alias` [newalias[=value] ]


---

### Q2.  List Files in Unix   

What do the following commands do:  
`ls`
> > List file information (alphabetically by default)

`ls -a`  
> > List information for all files including hidden

`ls -l`  
> > List long format file information

`ls -lh`  
> > List long format file information with 'human-readable' file sizes (e.g. 1K, 124M, 5G)

`ls -lah`  
> > List human-readable long format information for all files including hidden

`ls -t`  
> > List file information sorted by modification time

`ls -Glp`  
> > List long format file information excluding group membership and including file-type

---

### Q3.  More List Files in Unix  

Explore these other [ls options](http://www.techonthenet.com/unix/basic/ls.php) and pick 5 of your favorites:

List Option | Output
------------ | -------------
 `ls -R` | List contents recursively (all in current directory and below)
 `ls -S` | Sort by file size
 `ls -u` | Sort by last access time
 `ls -U` | Unsorted; list in directory order
 `ls -latr` | List all files in long form ordered by reverse time-modified (recently modified at bottom; good for very long lists)


---

### Q4.  Xargs   

What does `xargs` do? Give an example of how to use it.

> > Apply a command to a sequence of input items received via pipe.  
```bash
$ echo {1..6}
1 2 3 4 5 6

$ echo {1..6} | xargs -n 2 echo "By Twos:"
By Twos: 1 2
By Twos: 3 4
By Twos: 5 6
```
