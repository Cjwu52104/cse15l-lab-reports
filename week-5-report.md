### Using the grep Command in Git Bash

## 1.) Search recursively with -r 
**-r makes grep search recursively through all directories and files in the current working directory**

![image](/assets/report-3/first-r.PNG)

As you can see, it searched through everything in the `skill-demo-1` directory and found all the files containing the string "Lucayans".

![image](/assets/report-3/second-r.PNG)

None of the files in `skill-demo-1` contain the string "testing123", so it returns nothing.


## 2.) Ignore case distinctions with -i
**-i ignores case when searching for a specific string, so any sequence that matches the letters will return**

![image](/assets/report-3/first-i.PNG)


![image](/assets/report-3/second-i.PNG)

*Note: "lucayans" and "thirtieth street station" do not actually exist in any files within written_2. This command without -i would return nothing.*

## 3.) Listing only filenames with -l
**-l lists only the names of the files containing the string(s)**

![image](/assets/report-3/first-l.PNG)

![image](/assets/report-3/second-l.PNG)

*Note: this is useful for commonly recurring strings that will return a lot of files*

## 4.) show only the matching part of a line with -o

![image](/assets/report-3/first-o.PNG)

![image](/assets/report-3/first-o.PNG)

*Note: this is useful when searching for things like prefixes or suffixes that would appear in many different words.*

All command information was found using `grep --help` in bash, no external sources were used.
