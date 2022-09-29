# Lecture Note 5 (201933966_양시훈)
## 2022.09.29
---
### I/O Redirection 
**cat** : 'cat' displays the content of a text file.
**>** : You can redirect ouput using this.
*>>** : '>>' appends ouput to an existing file or create and write to a new file.
```sh
$ ls 0lh > file_list.txt
$ cat file_list.txt
$ ls -lh >> file_list.txt
```

**<** : You can redirect input from a file using "<"
\[tip] : You can also mix "<" and ">" together in a single line.
```sh
$ sort < words.txt > sorted_words.txt 
```

**|** : Pipeline("|") feeds output of previous command to input of next command.
```sh
$ ls -lh | less
```

### Expansion
Special characters expand its meaning when given to shell commands.
```sh
$ echo print out the text
$ echo * // *output the current directory's files* 
$ echo ~ // *output the current user's home directory
```
\[tip]
**Backslash(\)** : It can be usde to ignore line change in commnand "enter" to enter a long command in multiple lines.

### Permission
**Files and directories have a permision assigned differently to** ***owner***/***group***/***other***
- r : Read
- w : Write
- x : Execute
**chmod** : changes permission
-> Each permission of three objects(owner,group,others) is shown by binary number
-> ex) 6 = 110 = rw- 
```sh
$ chmod 600 some_file
```

\[tip] 
**history** : See previous command history.
```sh
$ history>history_command.txt
$ cat history
```













