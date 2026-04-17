## *Basics of Linux:


## **Lesson 1: Basic commands to navigate directories

1. **`pwd`** to know in which directory you are working presently.

2. Now lets create a new directory. To do so enter the below command
**`mkdir -v dir1`**

You will see an output like this: **"mkdir: created directory dir1"**
## ***Note: It is not necessary to use "-v" you can use mkdir dir1. But here "-v" tells us what we did(mkdir: created directory dir1).

3. Lets say we want to create more than one directory instead of invoking mkdir multiple(three) times-like.
**`mkdir -v dir2`**
**`mkdir -v dir2/dir3`**
**`mkdir -v dir2/dir3/dir4`**

you can simply use **`mkdir -vp dir2/dir3/dir4`**

**"-p"** option will create parent directories for "dir4" as needed. In this case,it creates dir2,dir3 automatically.Now we have created 4 directories.How to view them?

To view type 'ls' and press enter
**`ls`**
listed dir1 dir2 as directory content right? But where did other 2 directories go. Because other 2 directories were created inside dir 2. you need to use "complex" command to view them. Try this:
**`ls -R`**

**-R** stands for recursive.

Now lets go inside the new directory dir2. For this type:
**`cd dir2`**

you have changed to dir2 Now confirm this location by using previously learned pwd command.To move into next directory dir3

**`cd dir3`**

4. **`cd ..`** will move to parent directory.i.e dir2. or it goes one directory back.

5. Now type, **`cd -`** will move you to previous working directory i.e dir3

6. A simple **`cd`** will move to the your home directory.

That's it.You have successfully completed lesson1 Now to start next lesson.

## ** Lesson 2: Create files, display contents and stats

During Lesson1,you have learned how to create directories.

Lets learn to create a new file,

1. **`touch file1.txt`** and press enter key and read on :)

**touch** command will create a new file or change time stamp of an existing file. 

2. **`touch file2.txt`** will create an empty new file ,if the file is not already exists. 

3. To view directory contents ,you can also use: **` dir`** . **dir** is used to list directory contents.

4. To clear a screen,the command is **`clear`**

5. Let's print some message on the terminal, **`echo "hello"`**

The message will get printed on the cmd screen.🥳

6. Lets redirect the message to a new file instead of screen.
**`echo "hello" > hello.txt`**

## ***Note: To append data you must use >> not just >

**`echo "linux" >> hello.txt`**
**`echo "world" >> hello.txt`**

7. To view the file content ,do **`cat hello.txt`**
**cat** is used to display the entire file content.

8. To view only first two lines from the file **`head -2 hello.txt`**
By default,**head** will display the first 10 lines when you run,**`head hello.txt`**

9. Now how to view last two lines?.Its simple,use **tail**
**`tail -2 hello.txt`**
Thus **head** will be used to display **lines from begining** and **tail** will be used to display **last few lines.** As with head **`tail hello.txt`** by default will display last 10 lines from the line.

10 Lets check some stats of the files and directories we have create so far.
**`stat hello.txt`**
carefully examine few important fields the output. 

![Stat example](img/stat.png)

-> The first line shows the **filename** .second line says its a **regular file** with size as **18.**
-> Third line shows **Inode** number and no.of **links** to that inode.
-> Fourth one,says **owner(Uid),group(Gid)** who has read-write permission but other have read permission. Final three lines show **access,modified and change time.**. They mean:

| Term     | Description |
|----------|------------|
| Access   | When the file was last accessed/read |
| Modified | When the contents were last modified/written |
| Change   | Changes to file metadata (e.g., permissions) |


Now lets do a **stat** on directory.

**`stat dir1`**

![dir stat](img/dir1%20stat.png)
Compare the previous **stat** "hello.txt" output with "dir1",before you move. especially find out "dir1" type.