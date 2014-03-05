Eagle Preview Autogen
=====================

Git hooks to aid Eagle users in encouraging visual diffs. These scripts will run automatically when you commit any board changes, generating preview images and gerber files suitable for distribution. 

Requirements
------------
Currently, a Unix or Linux based OS, with Git, GerbV, and Eagle all placed in the system path. If you don't have Eagle in the path, you can edit the pre-commit file to add it in manually. 

For best usage, it's highly encouraged to also share your board on GitHub, since they have visual diffs between commits. 

Installation
------------

Copy the pre-commit and post-commit files into your .git/hooks folder. You'll also want to run `mkdir gerber-previews` and `git add gerber-previews`, since the script won't do this automatically 
