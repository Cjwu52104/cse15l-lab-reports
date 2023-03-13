### Lab Report 5: Find command options
Source used: [https://www.redhat.com/sysadmin/linux-find-command](https://www.redhat.com/sysadmin/linux-find-command)

1.) -iname

This option allows you to ignore case when using the find command.

![image](/assets/report-5/iname1.PNG)

Search for any file with the word "history" at the end, whether it was capitalized or not.

![image](/assets/report-5/iname2.PNG)

Search for a .txt file named "vallarta-history" regardless of case.

*Note: useful when you do not remember the capitalization of a file, or the capitalization system of your project is not consistent.*

2.) -exec

This option allows you to basically run multiple commands in a single command. In this case, I used the find command, then grep on the results of this find command.

![image](/assets/report-5/exec1.PNG)

Search for only .txt files containing "lucayans" (case ignored).

![image](/assets/report-5/exec2.PNG)

Search for a file named "Vallarta-History.txt" and then whether it contains the string "lucayans" (case ignored).

*Note: this option is very useful for getting more specific results (i.e. using grep on only certain files in your project)*

3.) -type

This allows you to search for all instances of a specific type, like files or directories.

![image](/assets/report-5/type1.PNG)

Search for all files in the current directory (response shortened to save space).

![image](/assets/report-5/type2.PNG)

Search for all subdirectories in the current directory.

*Note: this command may be useful when there are few instances of a certain type, or you are unsure whether a file/directory exists.*

4.) -empty

This allows you to search for only empty files in the specified directory.

![image](/assets/report-5/empty1.PNG)

Searches for all empty files in skill-demo1-data (there are none initially, so it does not return anything).

![image](/assets/report-5/empty1.PNG)

After adding an empty file to skill-demo1-data, the find -empty command now returns that file.

*Note: Handy when cleaning up a project with unnecessary empty files.*
