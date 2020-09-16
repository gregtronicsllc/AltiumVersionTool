# AltiumVersionTool

Welcome to the Altium version tool!  I created this tool to help me with with circuit designs using Altium.  I am not positive on the current state of things but previously with Altium you needed to copy and redo all your folder for revisions and I found it very cumbersome.  Aside from copying you would have to rename and relink things.  That's where this Python Script comes in.

# Software Notes

This tool was written in Python using version 3.7.0 on Windows 10.    
In the future I plan on writting this to reach more support for older Python and other operating systems. 

# In Development

1. Get released into pypi
2. Add more dynamic version finding.  Currently you have to have a format like ProjectName-A1 so it finds the current version. (See Folder Structure Below)  
3. Add a way to be able to start version controlling from a folder and files with no version on it 
4. Have a way to handle file names with different versions then the main version
5. Add support for library linking

# Current Folder Structure
You must have your project folder with the revision at the end (ProjectName-A1)
You must have a version in all the files names (Name-A1.SchDoc, Name-A1.PcbDoc).  The names don't have to be the same but all the versions should be the same.

# Usage

1. Run the script from any command prompt
2. Put in the absolute path of the folder you're revisioning to the next design.  This is the folder with your PcbDoc, PrjPcb, PrjPcbStructure, SchDoc, etc...
3. The script will analyze the folder and tell you what Version was found
4. The script will ask you if its a major/minor/custom revision.  
   a. A major revision is usually done after a design freeze and the board was made.  This will change the letter of the version
   b. A minor revision is usually done after any feature was complete and the design needs a change.  This will change the number
   c. A custom revision lets your name the version to whatever you want
5. The script will list all the items found and what was created

# Example

Coming soon
