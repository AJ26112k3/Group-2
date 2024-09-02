TASK-1

# Create the file with your first name
touch apurv.txt

# Add few lines without a text editor
echo "this is apurv" >> apurv.txt
echo " apurv is this" >> apurv.txt

# Add few more lines without a text editor
echo "bla blablal blala 3" >> apurv.txt
echo "bla bla bla bla 4v ftvtyvbgyugbyhn" >> apurv.txt
echo "bla bla abl 5" >> apurv.txt
echo "6 ugfbutitg6ifb9og" >> apurv.txt

# Rename the file with your last name
mv apurv.txt jha.txt

# Print the first 5 lines
echo "First 5 lines:"
head -n 5 jha.txt

# Print the last 5 lines
echo "Last 5 lines:"
tail -n 5 jha.txt

# Print lines 2 to 6 without using sed
echo "Lines 2 to 6:"
head -n 6 jha.txt | tail -n 5


TASK -2
# Step 1: Create a file with the first name in a text editor 
 vim saumya.txt &
# Step 2: Create a file with the last name in a text editor 
vim pathak.txt &
# Step 3: List out processes running in the system
ps aux
# Step 4: Identify and kill the process belonging to the first name 
ps aux | grep 'vim firstname.txt'
kill <PID>

TASK-3
1. Create a File Named saumya.txt
   Command:
   touch saumya.txt
   

2. Ensure That Only You Can Modify the File
   Symbolic Mode:
   chmod u=rw,go= saumya.txt
   
   Absolute (Numeric) Mode:
   chmod 600 saumya.txt
   

3. Create a New Group Named trusted
   Command:
   sudo groupadd trusted
  

4. Add Users veer and billu to the trusted Group
   Command:
   sudo usermod -aG trusted veer
   sudo usermod -aG trusted billu
   

5. Change the Group Ownership of the File to trusted
   Command:
   sudo chgrp trusted saumya.txt
  

6. Allow the trusted Group to Read and Modify the File
   Symbolic Mode:
   chmod g=rw saumya.txt
   
   Absolute (Numeric) Mode:
   chmod 660 saumya.txt
  

7. Allow All Other Users to Read the File
   Symbolic Mode:
   chmod o=r saumya.txt
  
   Absolute (Numeric) Mode:
   chmod 664 saumya.txt

TASK-4
# User Management and File Permission Task Documentation

1. Create a User with Your First Name
   Command:
   sudo useradd -m pathak
   This command creates a user named pathak with a home directory.

2. Create a System User for a Service with Your Last Name
   Command:
   sudo useradd -r -s /usr/sbin/nologin pathak
   This command creates a system user named pathak for service purposes, with no interactive login shell.

3. Remove Home Directory Information for the Last Name User
   Remove the existing home directory if it exists:
   Command:
   sudo rm -rf /home/pathak
   This command deletes the user's home directory if it exists.
   
   Update the user’s home directory to `/nonexistent`:
   Command:
   sudo usermod -d /nonexistent pathak
   This command sets the user’s home directory to `/nonexistent`.

4. Remove Login Shell for the Last Name User
   Command:
   sudo usermod -s /usr/sbin/nologin azeem
   This command removes the login shell for the user by setting it to `nologin`.

5. Create User Rahul and Ensure a Default File `file1` is in His Home Directory
   Create the user:
   Command:
   sudo useradd -m sanya
   This command creates the user sanya with a home directory.
   
   Create the file `file1` in sanya's home directory:
   Command:
   sudo touch /home/sanya/file1
   This command creates an empty file named `file1` in sanya's home directory.
   
   Set the correct ownership for the file:
   Command:
   sudo chown sanya:sanya /home/Rahul/file1
   This command sets the ownership of `file1` to the user sanya.
About
No description, website, or topics provided.
Resources
 Readme
 Activity
   

