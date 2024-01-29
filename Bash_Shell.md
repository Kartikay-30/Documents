 **Bash Shell Scripting**

![](https://lh7-us.googleusercontent.com/7ibztAUH9YGUTbFhsy2gfL0QRW75HHbUCIMa-s_-c5ganCn1i6Xoh6gv5d2GjtDrnxw-_9vf91nk3J8pW2At9MQERlZm_hJJWbzUwqPBJUlQDha3IsC_EE1JxHEuWtUo0oIxWFgvtALWBvdL00hSTA)  

![](https://lh7-us.googleusercontent.com/mVhKrK79bHLqPTGIjd3FND9OhxbtgPJRxMc7-BclQqFBhfyd4QBVYSVasTLG0Bw_ilGsAEVqBo1xZMl-xbXn3B40tcJACkLw1RzT89bc9Wn4Io3hun2ux2P7-G4wJB8Vzb0Q5Yz_HXeVXLlA6x7Gfg)

**By :- Kartikay** 

**Table of Content** 

[1. Introduction ](#introduction)

[Definition of Bash scripting ](#definition-of-bash-scripting)

[2. Advantages of Bash scripting ](#advantages-of-bash-scripting)

[➔ Automation ](#automation)

[➔ Portability ](#portability)

[➔ Flexibility ](#flexibility)

[➔ Accessibility ](#accessibility)

[➔ Integration ](#integration)

[➔ Debugging ](#debugging)

[3. How to Get Started with Bash Scripting ](#how-to-get-started-with-bash-scripting)

[4. Basic Bash commands ](#basic-bash-commands)


##

1. #  **Introduction**<a id="introduction"></a>

- Shell Scripting consists of a set of commands to perform a task.

- All commands execute sequentially.

- Tasks like file manipulation, program execution, user interaction, automation of tasks etc can be done by Shell Scripting.


## Definition of Bash scripting<a id="definition-of-bash-scripting"></a>

- A bash script is a file containing a sequence of commands that are executed by the bash program line by line. It allows us to perform a series of actions, such as navigating to a specific directory, creating a folder, and launching a process using the command line.

* By saving these commands in a script, we can repeat the same sequence of steps multiple times and execute them by running the script.

2. #  **Advantages of Bash scripting**<a id="advantages-of-bash-scripting"></a>

- ## **Automation**<a id="automation"></a>

* It allows us to automate repetitive task and processes, saving time and reducing the risk of errors that can occur with manual execution.

- ## **Portability**<a id="portability"></a>

* Shell scripts can run on various platforms and operating systems, like UNIX, Linux, macOS, and even Windows through the use of emulators or virtual machines.

- ## **Flexibility**<a id="flexibility"></a>

* Shell scripts are highly customizable and can be easily modified to suit specific requirements. 

- They can also be combined with other programming languages or utilities to create more powerful scripts.

* ## **Accessibility**<a id="accessibility"></a>

- Shell scripts are easy to write and don't require any special tools or software. 

* They can be edited using any text editor like ( nano,vim,vi ), and most operating systems have a built-in shell interpreter.

- ## **Integration**<a id="integration"></a>

* Shell scripts can be integrated with other tools and applications, such as databases, web servers, and cloud services, allowing for more complex automation and system management tasks.

- ## **Debugging**<a id="debugging"></a>

* Shell scripts are easy to debug, and most shells have built-in debugging and error-reporting tools that can help identify and fix issues quickly.

3. #  **How to Get Started with Bash Scripting**<a id="how-to-get-started-with-bash-scripting"></a>

- **Basic code**

```
kartik\@ubuntu:\~$ nano basic.sh
```
```
#!/bin/bash

echo "what is the number ?"
read k
echo "The number is :-" $k 
```
**OUTPUT**

```
kartik\@ubuntu:\~$ bash basic.sh
```
***
what is the number ?

23

The number is :- 23
***
**NOTE ➖**

- To write bash scripts we have to use some editors like (nano,vim,vi).

- To write a script we create a file using the above editors for e.g.- “**nano filename.sh**” here .sh is the extension to run the program.

- In above code “#!/bin/bash” named “**SHEBANG (#!)**”.It helps to execute the file using the Bash shell.

- Echo command is used to print the statement.

- Read command is used to enter the value.

- “$” means to find a specific value that we enter with the help of the read command.

- To run the program we have to write “**bash filename.sh**”, here .sh is the extension to run the program.
*******************************
*******************************
*******************************
- **Conditional Statement**

```
kartik\@ubuntu:\~$ nano condition.sh
```
```
#!/bin/bash

echo "Enter the number"

read num

if [ $num -lt 1000 ];
then
echo "Number is correct"
else
echo "Number is incorrect"
fi
```
**OUTPUT**

```
kartik\@ubuntu:\~$ bash condition.sh
```
***
Enter the number

12345

**Number is incorrect**
```
kartik\@ubuntu:\~$ bash condition.sh
```
Enter the number

123

**Number is correct**

*******************************
*******************************
*******************************

- **AND (&) Operator**
```
kartik\@ubuntu:\~$ nano and.sh
```
```
#!/bin/bash

echo "Now enter the details of user"
echo "Enter the username"
read user

echo "Enter the password"
read pass

if [[ ( $user == "Kartikay" **&&** $pass == "301224") ]];
then
echo "user is valid"
else
echo "user is invalid"
fi
```
**OUTPUT**

```
kartik\@ubuntu:\~$ bash and.sh
```
***
Now enter the details of user

Enter the username

kartikay

Enter the password

301224

**user is invalid**
```
kartik\@ubuntu:\~$ bash and.sh
```
Now enter the details of user

Enter the username

Kartikay

Enter the password

301224

**user is valid**
***
***************
***************
- **CASE Option**
```
**kartik\@ubuntu:\~$ nano case.sh**
```
```
#!/bin/bash

echo "Enter the assigned Single digit no. to check Employee details"

read val
case $val in

1)
echo "Name – Ram  Emp ID – 101 ";;
2)
echo "Name – Ramesh  Emp ID – 103 ";;
3)
echo "Name – Shyam  Emp ID – 102 ";;
4)
echo "Name – Vishal Emp ID – 104 ";;
5)
echo "Name – Aman  Emp ID – 105 ";;
*)
echo "Sorry! Invalid choice";;
esac
```
**OUTPUT**
**********
```
**kartik\@ubuntu:\~$ bash case.sh**
```
Enter the assigned Single digit no. to check Employee details

2

**Name – Ramesh  Emp ID – 103**
```
**kartik\@ubuntu:\~$ bash case.sh**
```
Enter the assigned Single digit no. to check Employee details

**\***

**Sorry! Invalid choice**

**********

4. #  **Basic Bash commands**<a id="basic-bash-commands"></a>

1)      cd: Change the directory to a different location.

2)      ls: List the contents of the current directory.

3)      mkdir: Create a new directory.

4)      touch: Create a new empty file.

5)      rm: Remove a file or directory.

6)      cp: Copy a file or directory.

7)      mv: Move or rename a file or directory.

8)      echo: Print text to the terminal.

9)      cat: Concatenate and print the contents of a file.

10)  read: This command helps us to print the value.
