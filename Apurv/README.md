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
 vim apurv.txt &
# Step 2: Create a file with the last name in a text editor 
vim jha.txt &
# Step 3: List out processes running in the system
ps aux
# Step 4: Identify and kill the process belonging to the first name 
ps aux | grep 'vim firstname.txt'
kill <PID>
