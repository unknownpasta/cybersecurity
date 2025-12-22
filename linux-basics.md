list: ls;
reverse: -r;
long list: -l; 
timestamp sort: -t; 
size sort: -s; 
change directory: cd; 
move up: cd ..; 
move down: cd ~
pwd: printing working directory
sudo; su: su creates a new shell as a root user whereas sudo executes root commands in the same shell

--------------------------------------------------------------------------------
when doing ls with the listing -l, it displays a longer line of code with al the information about the files. in the code the beginning would either have a '-' or a 'd', - meaning "file" and d meaning "directory" or folder. 

/* - rw-r--r-- 1 sysadmin sysadmin 647 Dec 20  2017 hello.sh */
the permission field is divided into three groups, "rw-r--r-- "
the first being "rw-" , being the owner
the second "r--" being the group
and he last "r--" being others.
when reading files, read is r, write is w and execute is x 
---------------------------------------------------------------------------------
to change file perms 'chmod' is used.
chmod [<SET><ACTION><PERMISSIONS>]... FILE
--------
in the SET part, it changes permission for:
u - User: The user who owns the file.
g - Group: The group who owns the file.
o - Others: Anyone other than the user owner or member of the group owner.
a - All: Refers to the user, group and others.
--------
in the ACTION part, it tells the code what to do.
+ - Add the permission, if necessary
= - Specify the exact permission
- - Remove the permission, if necessary
--------
in the permission part, you pick the permission you want to alter.
r - read
w - write
x - execute
---------------------------------------------------------------------------------
change file ownership
chown [OPTIONS] [OWNER] FILE
to use chown sudo is needed.
"sudo chown root hello.sh"
---------------------------------------------------------------------------------
VIEWING FILES
cat is used to view files in linux, cat being short for concatenate 
for longer files
head is used to view the topmost lines
while
tail is used to view the bottom-most lines
---------------------------------------------------------------------------------
CREATING DIRECTORIES and TEXT FILES
To create in Linux, we use:
mkdir //for directories

touch //for text files

To read the files we use:
cat

To update the files we use:
echo  - example//"echo "linux crud practice" >> notes.txt"

To delete:
rm    //for text files
rmdir    //for directories
rm -rf *    //to delete everything







