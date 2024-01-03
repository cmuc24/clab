# How to read file line by line in Bash

Source: <https://linuxhint.com/read_file_line_by_line_bash/>

How would you write a Bash script that can process a text file one line at a time.  First you need a syntax and approach to read the file line by line. The methods for this approach are shown in this tutorial.

Suppose, you have a file named **company.txt** which contents the company names. This file contains the following content.

```
Company.txt
Samsung
Nokia
LG
Symphony
iphone
```

### **Example -1: Reading file content from command line**

Suppose, you want to read the file, **company.txt**, line by line from the command line without **‘cat’** command. Run the following command to do the task. **while** loop will read each line from the file **company.txt** in each step and store the content of the line in **$line** variable which will be printed later.

\
 ![](https://linuxhint.com/wp-content/uploads/2018/06/r-1.png)

```bash
while read line; do echo $line; done < company.txt
```

### **Example -2: Reading file content using script**

Create a bash file and add the following code to read the content of a particular file. Here, an existing filename is stored in $filename** variable and **$n variable is used to keep the value of the line number of that file. Like previous example, **while** loop is used to read this file with line number.

```bash
#!/bin/bash
filename='company.txt'
n=1
while read line; do 
# reading each line 
echo "Line No. $n : $line"
n=$ ((n+1))
done < $filename
```

Run the following command to execute the script.
`readfile1.sh`

Run **‘cat’** command with **company.txt** file to display the original content of **company.txt** file.

`cat company.txt`

 ![](https://linuxhint.com/wp-content/uploads/2018/06/r1-1.png)

### **Example -3: Passing filename from the command line and reading the file**

Create a bash file and add the following script. This script will take the filename from the command line argument. First argument value is read by the variable $1 which will contain the filename for reading. If the file exists in the current location then **while** loop will read the file line by line like previous example and print the file content.

```bash
#!/bin/bash
filename=$1
while read line; do
# reading each line
echo $line
done < $filename
```

Run the above script with **employee.txt** file as argument value. The output will show the content of **employee.txt** file by removing extra space. You can show the original content of **employee.txt** file by using **‘cat’** command.

```bash
$ bash readfile2.txt employee.txt
$ cat employee.txt
```

 ![](https://linuxhint.com/wp-content/uploads/2018/06/r2-2.png)

### **Example – 4: Reading file by omitting backslash escape**

If you want to read each line of a file by omitting backslash escape then you have to use **‘-r’** option with read command in **while** loop.

```bash
#!/bin/bash
while read -r line; do
# Reading each line
echo $line
done < company2.txt
```

Create a file named **company2.txt** with backslash and run the following command to execute the script. The output will show the file content without any backslash.

 ![](https://linuxhint.com/wp-content/uploads/2018/06/r3-1.png)

You will need to read the file for many programming purposes. For example, you can search or match any particular content easily from any file by reading each line separately. So, it is an essential task for any programming. Some simple examples of reading file in bash script are shown in this tutorial. These will help you to get the idea of reading file content line by line using while loop in bash script and apply in your script more efficiently. For more information watch [the video](https://youtu.be/1JpkmqU5oko)!

### About the author

I am a trainer of web programming courses. I like to write article or tutorial on various IT topics. I have a YouTube channel where many types of tutorials based on Ubuntu, Windows, Word, Excel, WordPress, Magento, Laravel etc. are published: [Tutorials4u Help](https://www.youtube.com/channel/UCIa6d3QPq7Ulqz8Ha2WRf3A).

Source: <https://linuxhint.com/read_file_line_by_line_bash/>