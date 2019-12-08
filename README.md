One of the lesser known features of Nautilus is the ability to add scripts to run on files or folders. This is a simple script to open Jupyter in the selected folder in conda environment named 'default' 

# Usage guide

## Step 1
Download the script 'Jupyter' to 

    ~/.local/share/nautilus/scripts

## Step 2
Customise the script by replacing the conda environment 'default' to your own one by editing this line:

    exec x-terminal-emulator -e "bash -c -i 'eval $(conda shell.bash hook); conda activate default && jupyter notebook;exec $SHELL'"

## Step 3
Make the script executable:

    chmod a+x ~/.local/share/nautilus/scripts/Jupyter

***
### Right click on a file or folder to find 'Jupyter' under the menu option 'Scripts'. 