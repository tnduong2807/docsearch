# Week 5 Lab Report - Commands

## 3 interesting command-line options or alternate ways to use find:

**1.Use -name with extension or asterisk symbol to search for a specific file:**

`find -name "*chapter*"`

![](https://github.com/tnduong2807/docsearch/blob/main/Screenshot%20(57).png?raw=true)

The find -name with extension command could use find all files that end with specific extension. It's useful because it is save a lot of time to find files with the same name and we all love being lazy as programmers.

**2.Use -size to search for the files with specific size or weight:**

`find technical/ -size -2k`

![](https://github.com/tnduong2807/docsearch/blob/main/Screenshot%20(59).png?raw=true)

The find -size command could use find all the files with the specific size, for example find files that size less than 2 kilobytes. It is usefull because we could find all the files with specific size to find any kind of files knowing its' size.

**3.Use -type to search the files with specific type:**

`find technical/ -type d`

![](https://github.com/tnduong2807/docsearch/blob/main/Screenshot%20(58).png?raw=true)

The find -type command could use find all the files with the specific type, for examples find files that is the directory type. It is useful because we could find all the files with specific type to find any kind of files knowing its' types.

## 3 interesting command-line options or alternate ways to use less:

**1.Use -N to display the specified text file with line numbers:**

`less -N technical/*/chapter-1.txt`

![](https://github.com/tnduong2807/docsearch/blob/main/Screenshot%20(60).png?raw=true)

The less -N command could use display the specific text line with line numbers. It is useful becasue we could label the text line with line numbers and make it easier to locate a specific issue.

**2.Use -s to remove multuple blank lines from a text file into one black line:**

`less -s technical/*/chapter-1.txt`

![](https://github.com/tnduong2807/docsearch/blob/main/Screenshot%20(61).png?raw=true)

The less -s command could remove multiple blank lines and allow to show more contents in one screenful of that file. It is useful because it will make the contents of the file more readable and create a more clean version of that file.

**3.Use -X to leave the file contents in the terminal after quitting:**

`less -X technical/*/chapter-1.txt`

![](https://github.com/tnduong2807/docsearch/blob/main/Screenshot%20(62).png?raw=true)

The less -X command could leave the file contents on the terminal. It is useful because we can multitask with the contents on the terminal.

## 3 interesting command-line options or alternate ways to use grep:

**1.Use -c to display the count of number of matches:**

`grep -c "rheimatoid" technical/*/ar68.txt`

![](https://github.com/tnduong2807/docsearch/blob/main/Screenshot%20(63).png?raw=true)

The grep -c command is to display the number of lines that matches the given string or pattern. It is useful because we can find how many lines that contain the pattern in the contents of the files and know if the contents of the file have the keyword or not.

**2.Use -l to display the file names that have the contents matches the pattern:**

`grep -l "hiv" technical/biomed/*`

![](https://github.com/tnduong2807/docsearch/blob/main/Screenshot%20(64).png?raw=true)

The grep -l command is to display the files that contains the given string/pattern. It is useful because we could locate the files that contains the given string and it could save so much time to find the names of the files.

**3.Use -n to show the line number while displaying the contents that conatains the string:**

`grep -n "biomed" technical/biomed/*`

![](https://github.com/tnduong2807/docsearch/blob/main/Screenshot%20(64).png?raw=true)

The grep -n command is to show the line number of file with the line matched the given string. It is useful because we could locate the lines that conatins the given string in many different files that contains that given string and it could save so much time to find lines in differents files that have the given string.