These are several scripts that I wrote as a project for a UNIX administration course. They handle the following operations (with extensive error checking): 

1. Creating a new user
    Usage: create_user -l <username> -u <userID> -g <groupID> -i <GECOS> -d <homedir> -s <shell> 
    a. Create an entry in the passwd file
    b. Create a new home directory for the user
    c. Move contents of skel directory to the user's home durectory
    d. If all succeeds, add an entry to the log
2. Adding a new group
    Usage: add_group -n <name> -g <groupID>
    a. add entry to the group file 
    b. If all succeeds, add anentry to the log
3. Archiving an existing user  
   Usage: archive_user -l <username>
    a. Archive the home directory
    b. Remove user's entry from the passwd file
    c. If all succeeds, append entry to the log

