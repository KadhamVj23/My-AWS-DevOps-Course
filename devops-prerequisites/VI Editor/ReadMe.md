# **Console Based text Editors(VI Editor)**
In Linux we will be modifying many files so in these cases the console based editors come very handy, and there are many editors available like VI Editor, VIM, Nano.  

Here we will be discussing about VI editor it is one of most popular ones. 

VI Editors comes installed by default in most OS. Enter this command: vi file_name. For eg: vi index.html -> then the terminal opens the file. 

Then you will be inside VI editor. VI editor has 2 modes of operation:
1. Command Mode 
2. Insert Mode. 

In the vi editor when you open the file you are by default in the **Command Mode**, here you can issue commands to the file like copy or paste lines, or delete a line or a word, or to navigate between lines etc. But you CANNOT write the contents to the file.  

To write the content you need to switch the **INSERT MODE**. To switch to this mode type lower case **i**.  

Once you are in INSERT Mode you will be able to modify the files as you would normally. 

To switch back from INSERT Mode press **esc** key. 

Now lets see what commands are available in Command Mode. 

You can use the arrow commands to move around the editor or the keys: **“K,H,J,L”**  

**K** --> To go UP 

**H** --> To go LEFT 

**J** --> To go DOWN 

**L** --> To go RIGHT 


To delete a character press **X** . Typing **dd** deletes the entire line.  

To copy a line type **yy** and to paste it type **p** 

To scrollUp/Down press **CTRL+U** or **CTRL+D**

Typing in **“ : “** takes you to the prompt, where you can type commands.  

To save the changes made to the file and write the file to disk use **“ :w “** command. You can optionally specify the file name as well **“ :w filename “**

To discard any unsaved chnages made to the file type **“ :q “** command 

To save changes and quite tpye in **“ :wq “** command. 

How do you find the stuff in the file: 

For eg we want to find the word “of” in the file then you need to type the command **“ /of”**  when you do this all the occurrences of the word “of” are highlighted and the cursor is positioned at that location. To move the cursor to the rest of the occurrences press the **“n”** key. 

You can continue to press “n” key to move the cursor to all future occurrences. 

**FIND - > /of**  

To move the cursor to other occurrences, **press -> n**

Below are the commands screenshots:
![Vi Editor Commands](screenshots/vi%20editor%20commands.png)
![Copy & Paste](screenshots/Copy&Paste.png)
![Delete Command](screenshots/Delete.png)
![Move Around](screenshots/Move%20Around.png)