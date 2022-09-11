# Kali Linux Commands
## history	
* This command is used to print the bash history of the current user.
## free
* It gives the information about the available RAM and the total used and available spaces of physical memory and swap memory with buffer used by Kernal.
## vi
* It is a screen editor used to edit the file.
## sort
* It sorts the content of a text file line by line.
## more
* It is used to display output in the terminal, one page at a time.
## less
* It is used to view the file instead of opening the file.
## date
* This command is used to display the system date and time.
## cal
* It will display a formatted calendar of the current month.
## whoami
* It will print the active user ID.
## pwd
* It stands for "Print Working Directory" which prints the name of the working directory.
## ls
* It is used to list out all the hidden files of a directory with -an attribute.
## users
* It will display login names of the user currently logged in to the system.
## uptime
* It will return you the time for which the system has been up.
## uname
* It prints information about the current system.
## rm
* It is used to delete files and directories.
## mv
* This command moves, or renames, files, and directories on your file system.
## cp	
* It is used to copy files.
## cat	
* It is used to create single or multiple files, view contained file, concatenate files, and redirect output in terminal or files.
## mkdir
* It is used to create directories.
## cd	
* It is used to change or switch the current working directory.

# Category 1:
##  **General**
* Let’s begin with the general commands first.

# 1. uname: 
* **Get detailed info on your system specifications with this command. Great place to start familiarizing yourself with Kali User Interface.**
 <img width="365" alt="image" src="https://user-images.githubusercontent.com/104230071/189521607-cf3f9a7f-92df-4151-82b9-98d755825e4f.png">
 
  # 2.Pwd: 
 
 * **This command prints the name of the working directory.**
<img width="241" alt="image" src="https://user-images.githubusercontent.com/104230071/189524746-67103d2c-46e0-4bfa-9d18-c31e1824ea9e.png">

 
 * A convenient way of showing the directory you’re working in. Especially useful for novices since Kali Linux has a command shell where it’s easy to get lost when you’re in the middle of something complicated.
 # 3. ls: 
 * **This command Displays what each file contains and the directories they’re stored in. An easy way to view all the contents (files) contained in a directory**
 <img width="382" alt="image" src="https://user-images.githubusercontent.com/104230071/189524812-ef957616-2d0f-4603-96ae-70789b8bdf30.png">

 
 * The -l  flag details each category, other than that, you can use -an attribute.
 # 4. history: 
 * **Get to know all the previously used commands and attributes with history command. It lists all the previous commands you entered (stored in bash shell).**
 <img width="269" alt="image" src="https://user-images.githubusercontent.com/104230071/189524844-f45b6e3f-c04d-4569-a2dd-6624d327a058.png">


# 5. macchanger:macchanger changes your mac address, essentially changing your identity.
<img width="377" alt="image" src="https://user-images.githubusercontent.com/104230071/189524884-14d0b23f-4530-4ed8-8705-96b67c2fcf5e.png">


# 6. ifconfig :
* **ifconfig <=> interface configuration.**
* Lets you view current network interface settings and configure them.
<img width="370" alt="image" src="https://user-images.githubusercontent.com/104230071/189524945-ddd3f786-916b-4ab2-8681-0be8cf5205dd.png">


# 7. echo: 
* **It’s like the basic print function you learned in GW basic. Prints any text to where you direct it to.**
* echo > [file name]  prints the copied text in a new file.
* echo >> [file name]  prints the copied text to an existing file.
* Using echo  without a ‘>’ will automatically create a new file for the text.
<img width="316" alt="image" src="https://user-images.githubusercontent.com/104230071/189525153-c035db96-29c8-4a90-b587-51d8ad61ae3a.png">


# 8. cat: 
* **Lets your read files and link them together, exchange their contents, etc.**
<img width="401" alt="image" src="https://user-images.githubusercontent.com/104230071/189523353-c9373369-386a-4fbd-a59b-167ec5479451.png">

# 9. Clear: 
* **Pretty self-explanatory, clears the terminal screen, and lets you fill it anew.**
<img width="235" alt="image" src="https://user-images.githubusercontent.com/104230071/189523522-626d14a3-a4a0-4a0a-8730-a94a05b85664.png">

# Category 2:
* **Manipulation commands:**
* Manipulation commands let you make modifications to files and their content.s

# 10. mkdir:
* **Creates a new directory.**

* To create a directory under Desktop called folder1, open a terminal and type this:
<img width="296" alt="image" src="https://user-images.githubusercontent.com/104230071/189523689-79ad51c4-3614-48bf-ac4f-6f66b4a6f754.png">

# 11. cd:
* **changes the directory you’re working in. Very commonly used, and a very convenient way to shift directories.**
<img width="344" alt="image" src="https://user-images.githubusercontent.com/104230071/189523854-0ed8898c-3d24-4935-9f09-ba2f8b5e2ca0.png">

# 12. cp:
* **Serves the basic copy-text/something purpose. Use this to copy one or more files to a location of your choice. You can pretty much move entire directories with this command.**
<img width="398" alt="image" src="https://user-images.githubusercontent.com/104230071/189523972-0ed436cc-44d7-444b-aee2-209a5d65286d.png">

# 13. mv:
* **This command moves files between directories.**
* <img width="390" alt="image" src="https://user-images.githubusercontent.com/104230071/189524038-92460257-51ca-4ce3-b18e-7b7715ba9126.png">

# 14. rm:
* **Very basic yet essential command, rm removes highlighted texts.**
<img width="386" alt="image" src="https://user-images.githubusercontent.com/104230071/189524121-5f07203f-7aa5-42b3-aa97-dd98e10090da.png">

# 15. more:
* **more gives you bird’s eye view of the contents of a file.**
<img width="393" alt="image" src="https://user-images.githubusercontent.com/104230071/189524179-24f974e9-8432-41fb-95fe-b2eda00f4706.png">

# 16. less:
* **does everything that more does, just saves you some RAM while it’s at it. Shows you what’s going on with a certain file, except it doesn’t completely load it.**
<img width="382" alt="image" src="https://user-images.githubusercontent.com/104230071/189524289-6f784ff3-15bf-455b-a024-0fa34aa11b3c.png">

# 17. sort:
* **see information sorted, to see contents in a certain orderly arrangement. Use -r switch, to sort the contents in reverse order.**
<img width="395" alt="image" src="https://user-images.githubusercontent.com/104230071/189524397-d0c99a03-0813-413b-8096-194aeb1d0558.png">

# 18. vi: 
* **Short for the visual editor.**

This is a text editor you type filenames into. Type your text like vi(filename). This editor has two modes: command and insert. You are in command mode by default. To enter the insert mode, type i then type Esc to exit. Exit vi by typing ‘:wq’
<img width="514" alt="image" src="https://user-images.githubusercontent.com/104230071/189524638-503bd192-f139-4c35-920a-bfc33e748c62.png">










