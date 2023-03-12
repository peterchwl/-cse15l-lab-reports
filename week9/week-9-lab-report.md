# Week 9 Lab Report
In this week's lab report, students are required to go back to a previous lab or lab report and go more in-depth on the task. I will complete Lab Report 3 with a different command than the one I investigated initially.

In the original Lab Report 3, I focused on the grep command. In this Lab Report, I will focus on the the find command.

&nbsp;
## **Command 1: "-type"**
___
-type: The find command in bash is used to search for files or directories in a specified location. The -type option is used to specify the type of file or directory to search for.

**Example 1:**

Command:

(Inside path "/home/linux/ieng6/cs15lwi23/cs15lwi23avu/skill-demo1-data/written_2/non-fiction/OUP")
```
find -type d
```
Output:
```bash
.
./Abernathy
./Berk
./Castro
./Fletcher
./Kauffman
./Rybczynski
```

Adding "d", every directory and subdirectories within the directories are listed. This is useful as it allows users to search for every directory within a directory.

**Example 2:**

Command:

(Inside path "/home/linux/ieng6/cs15lwi23/cs15lwi23avu/skill-demo1-data/written_2/non-fiction/OUP")

```bash
find -type f
```
Output:
```
./Abernathy/ch1.txt
./Abernathy/ch14.txt
./Abernathy/ch15.txt
./Abernathy/ch2.txt
./Abernathy/ch3.txt
./Abernathy/ch6.txt
./Abernathy/ch7.txt
./Abernathy/ch8.txt
./Abernathy/ch9.txt
./Berk/CH4.txt
./Berk/ch1.txt
./Berk/ch2.txt
./Berk/ch7.txt
./Berk/test.txt
./Castro/chA.txt
./Castro/chB.txt
./Castro/chC.txt
./Castro/chL.txt
./Castro/chM.txt
./Castro/chN.txt
./Castro/chO.txt
./Castro/chP.txt
./Castro/chQ.txt
./Castro/chR.txt
./Castro/chV.txt
./Castro/chW.txt
./Castro/chY.txt
./Castro/chZ.txt
./Fletcher/ch1.txt
./Fletcher/ch10.txt
./Fletcher/ch2.txt
./Fletcher/ch5.txt
./Fletcher/ch6.txt
./Fletcher/ch9.txt
./Kauffman/ch1.txt
./Kauffman/ch10.txt
./Kauffman/ch3.txt
./Kauffman/ch4.txt
./Kauffman/ch5.txt
./Kauffman/ch6.txt
./Kauffman/ch7.txt
./Kauffman/ch8.txt
./Kauffman/ch9.txt
./Rybczynski/ch1.txt
./Rybczynski/ch2.txt
./Rybczynski/ch3.txt
```

Adding "f", every file that is not a subdirectory or special file within the directory and its subdirectories is listed. This is useful as it allows users to search for every file within a directory and the subdirectories within the directory, making finding a file more thorough and easier.

**Citation:**
To find this command I asked ChatGPT. My prompt was: "give me the easiest/simplest command-line options to use with find". I made sure my commands worked with command line after seeing the results.

&nbsp;
## **Command 2: "-name"**
___
-name: This command finds all files with a specified filename in the specified directory and its subdirectories.

**Example 1:**

Command:

(Inside path "/home/linux/ieng6/cs15lwi23/cs15lwi23avu/skill-demo1-data/written_2/non-fiction/OUP")

```bash
find -name "ch2.txt"
```
Output:
```
./Abernathy/ch2.txt
./Berk/ch2.txt
./Fletcher/ch2.txt
./Rybczynski/ch2.txt
```

In bash, this command finds all the text files named "ch2.txt" in the OUP directory, including its subdirectories. This is useful as it allows users to easily find if a file exists in a directory, and where it is within a directory as the path is given.

**Example 2:**

Command:

(Inside path "/home/linux/ieng6/cs15lwi23/cs15lwi23avu/skill-demo1-data/written_2/non-fiction/OUP")

```bash
find -name "ch5.txt"
```
Output:
```
./Fletcher/ch5.txt
./Kauffman/ch5.txt
```

In bash, this command finds all the text files named "ch5.txt" in the OUP directory, including its subdirectories. This is useful as it allows users to easily find if a file exists in a directory, and where it is within a directory as the path is given.

**Citation:**
To find this command I asked ChatGPT. My prompt was: "give me the easiest/simplest command-line options to use with find". I made sure my commands worked with command line after seeing the results.

&nbsp;
## **Command 3: "-size"**
___
-size: Use this command to search for files of a specific size.

**Example 1:**

Command:

(Inside path "/home/linux/ieng6/cs15lwi23/cs15lwi23avu/skill-demo1-data/written_2/travel_guides/berlitz2")

```bash
find -size +100k
```
Output:
```
./Canada-WhereToGo.txt
./China-WhereToGo.txt
./Portugal-WhereToGo.txt
```

In bash, this command finds all the text files that have a size greater than 100 kilobytes. This is useful as it allows users to easily find files based on their sizes, allowing users to identify large and small files in a directory.

**Example 2:**

Command:

(Inside path "/home/linux/ieng6/cs15lwi23/cs15lwi23avu/skill-demo1-data/written_2/non-fiction/OUP")

```bash
find -size +200k
```
Output:
```
./Canada-WhereToGo.txt
```

In bash, this command finds all the text files that have a size greater than 200 kilobytes. This is useful as it allows users to easily find files based on their sizes, allowing users to identify large and small files in a directory.

**Citation:**
To find this command I asked ChatGPT. My prompt was: "give me the easiest/simplest command-line options to use with find". I made sure my commands worked with command line after seeing the results.

&nbsp;
## **Command 4: "-maxdepth"**
___
-maxdepth: This command is used to limit the depth of the search. For example, to search for files only in the current directory (not in any subdirectories), you can use the command.

**Example 1:**

Command:

(Inside path "/home/linux/ieng6/cs15lwi23/cs15lwi23avu/skill-demo1-data/written_2/non-fiction")

```bash
find -maxdepth 3 -type f
```
Output:
```
./OUP/Abernathy/ch1.txt
./OUP/Abernathy/ch14.txt
./OUP/Abernathy/ch15.txt
./OUP/Abernathy/ch2.txt
./OUP/Abernathy/ch3.txt
./OUP/Abernathy/ch6.txt
./OUP/Abernathy/ch7.txt
./OUP/Abernathy/ch8.txt
./OUP/Abernathy/ch9.txt
./OUP/Berk/CH4.txt
./OUP/Berk/ch1.txt
./OUP/Berk/ch2.txt
./OUP/Berk/ch7.txt
./OUP/Berk/test.txt
./OUP/Castro/chA.txt
./OUP/Castro/chB.txt
./OUP/Castro/chC.txt
./OUP/Castro/chL.txt
./OUP/Castro/chM.txt
./OUP/Castro/chN.txt
./OUP/Castro/chO.txt
./OUP/Castro/chP.txt
./OUP/Castro/chQ.txt
./OUP/Castro/chR.txt
./OUP/Castro/chV.txt
./OUP/Castro/chW.txt
./OUP/Castro/chY.txt
./OUP/Castro/chZ.txt
./OUP/Fletcher/ch1.txt
./OUP/Fletcher/ch10.txt
./OUP/Fletcher/ch2.txt
./OUP/Fletcher/ch5.txt
./OUP/Fletcher/ch6.txt
./OUP/Fletcher/ch9.txt
./OUP/Kauffman/ch1.txt
./OUP/Kauffman/ch10.txt
./OUP/Kauffman/ch3.txt
./OUP/Kauffman/ch4.txt
./OUP/Kauffman/ch5.txt
./OUP/Kauffman/ch6.txt
./OUP/Kauffman/ch7.txt
./OUP/Kauffman/ch8.txt
./OUP/Kauffman/ch9.txt
./OUP/Rybczynski/ch1.txt
./OUP/Rybczynski/ch2.txt
./OUP/Rybczynski/ch3.txt
```

In bash, combining maxdepth with "-type f" gives us all of the files in the nonfiction directory at a depth of 3, meaning it only finds files that are up to 2 subdirectories in the original directory (since a depth of 1 is the current directory). This is useful as it allows users to find a file within a specific directory depth within the current directory.

**Example 2:**

Command:

(Inside path "/home/linux/ieng6/cs15lwi23/cs15lwi23avu/skill-demo1-data/written_2")

```bash
find -maxdepth 2 -type d
```
Output:
```
.
./non-fiction
./non-fiction/OUP
./travel_guides
./travel_guides/berlitz1
./travel_guides/berlitz2
```

In bash, combining maxdepth with "-type d" gives us all of the directories in the written_2 directory at a depth of 2, meaning it only finds directories that are up to 1 subdirectories in the original directory (since a depth of 1 is the current directory). This is useful as it allows users to find a directory within a specific directory depth within the current directory.

**Citation:**
To find this command I asked ChatGPT. My prompt was: "give me the easiest/simplest command-line options to use with find". I made sure my commands worked with command line after seeing the results.
