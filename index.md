# Week 5 Lab Report - Commands

## 3 interesting command-line options or alternate ways to use find:
1. Use -name with extension or asterisk symbol to search for a specific file:

`find -name "*chapter*"`

![](https://github.com/tnduong2807/docsearch/blob/main/Screenshot%20(57).png?raw=true)

The find -name with extension command could use find all files that end with specific extension. It's useful because it is save a lot of time to find files with the same name and we all love being lazy as programmers.

2. Use -size to search for the files with specific size or weight:

`find technical/ -size -2k`

![](https://github.com/tnduong2807/docsearch/blob/main/Screenshot%20(59).png?raw=true)

The find -size command could use find all the files with the specific size, for example find files that size less than 2 kilobytes. It is usefull because we could find all the files with specific size to find any kind of files knowing its' size.

3. use -type to search the files with specific type:

`find technical/ -type d`

![](https://github.com/tnduong2807/docsearch/blob/main/Screenshot%20(58).png?raw=true)

The find -type command could use find all the files with the specific type, for examples find files that is the directory type. It is useful because we could find all the files with specific type to find any kind of files knowing its' types.



