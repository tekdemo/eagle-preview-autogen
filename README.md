Eagle Preview Autogen
=====================

Git hooks to aid Eagle users in encouraging visual diffs. These scripts will run automatically when you commit any board changes, generating preview images and gerber files suitable for distribution, and can include them in every commit. By default, only the images are added, to simplify changelogs.

If ImageMagick is installed, it also generates a visual diff of board changes, and includes those into your commit as well. This technique is based off Evil Mad Science Lab's [Visual Diff guide](http://www.evilmadscientist.com/2011/improving-open-source-hardware-visual-diffs/).

You can see sample images that this will generate at this [this commit](https://github.com/tekdemo/eagle-preview-autogen/commit/d607463c2a51fec488ca56b69db318d3f668e53e)


Requirements
------------
Currently, a Unix or Linux based OS, with Git, GerbV, and Eagle all placed in the system path. If you don't have Eagle in the path, you can edit the pre-commit file to add it in manually. 

ImageMagick is optional, but handy. 

For best usage, it's highly encouraged to also share your board on GitHub, as their visual diff tool is stellar as well.


Installation
------------

Copy the pre-commit and post-commit files into your .git/hooks folder, and optionally edit the pre-commit file to include any pathnames.  You'll also want to run `mkdir gerber-previews` and `git add gerber-previews`, since the script won't do this automatically.
