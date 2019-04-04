# Command Line

## Commands 
[Note that these commands are Unix Code]

`pwd` - show the current (or "working") directory. Stands for "print working directory"

`ls` - show the files and folders in the working directory. I think of it as standing for "list stuff," but it's probably just short for "list."

- `ls -1` - show the files and folders in a nice vertical column.

`cd` - move to a directory, i.e. `cd Desktop` will move to the "Desktop" folder. Some special cases:

- `cd ..` - go to the directory above
- `cd ~` go to your "home" directory, i.e. /Users/<yourname>
- `cd` (by itself) also goes to the home directory
- `cd -` go to the last directory you were in before the current
- `cd ../..` travel two directories up
- `cd Documents/thesis-drafts` move two directories, from the home folder to "thesis-drafts," skipping "Documents"

`touch <filename>` - Create an empty text file named <filename> in your current directory.

`code <filename>` - Open file in VS Code (and create it, if it does not already exist).

`mkdir <folder name>` - Create a directory named `<folder name>` in the current working directory.

`echo <some text>` - Print out any text you give it. Often used with a redirect to add text to a file.

`cat <filename>` - Print the contents of a file to the screen, in this case the contents of `<filename>`

`>` - Redirects printed output to a text file, as in `echo "this is some text" > hello.txt`

`>>` - Redirect and append. If there's already a file with text in it, this command will add that text to the file without destroying and recreating it.

`|` - Pipe symbol. Takes output from one command and uses it as input for another command.

`less <filename>` - Print out the contents of a file in a paginated form. Use `<Control-v>` and `<Alt-v>` (or `<Command-v` and `<Option-v>`) to move up and down. Press `q` to quit.

`head <filename>` - Print the first section of a file

`tail <filename>` - Print the last section of a file

`wc -l` - Takes input and returns the number of lines in that input, as in `cat <filename> | wc -l`

`sort` - Arrange lines in a file in numeric and alphabetical order.

`uniq` - Remove duplicate lines from input, as in `cat <filename> | uniq`. To show the duplicate files, use `uniq -d`. Often most useful after using `sort`, since it only removed duplicates that are next to one another.

`mv` - Move or rename a file. For example, `mv file1 file2` will rename `file` to `file2`. You can also specify another destination, so that `mv file1 ~` will move file1 to the home folder without renaming it.

`rm <filename>` - Permanently remove a file from your computer.


Also check out [other useful commands](other-commands.md)

## Glossary

### Synonyms for the command line

*bash* - the programming language used in the command line. (Yes, we tricked you, you're already programming!) Short for "Born Again SHell," for reasons people on the internet will happily tell you about.

*cli* - "Command Language Interpreter," this is a super technical term for the command line used to impress everyone around you.

*the shell* - The part of an operating system that interacts with a human. Technically, anything you do in a graphical interface is also in a shell, but in practice this is just another synonym for the command line.

*the terminal* - Particularly used to refer to the command line on OSX. This term made more sense when universities used mainframes and every computer was only a terminal.

### Other Terms

*argument* - in the command line, an argument is an item or parameter that you give a program when you start it. For instance, if you 

*command* - a specific task or function given to a computer application (Terminal or Bash in this tutorial) to perform some kind of task or function. At first it may seem like aribtrary letters are pulled out of thin air to enact some sort of magic. In fact, these commands (`mkdir`, `ls`, etc.) have been written by people to fulfill express functions. Options (see below) were developed for specific commands based on the commands' functions. Most users only need a small set of the commands that come pre-installed in their command line interface to complete their desired tasks.

*flag* - otherwise known as an *option* or *switch*, a flag provides additional information for how you wish a program to run. For instance, when executing the command `grep`, you may want to add the flag `-i` to ignore capitalization. If you wish to know what flags belond to particular commands, you can check the m

*GUI* - "Graphical User Interface." Pronounced "gooey," like delicious gooey chocolate. Basically, anything on a computer that isn't in the command line. All familiar elements of day-to-day computer tasks such as images, windows, prompts, buttons, and progress bars are part of the GUI. The way most people interact with computers. Some tasks can only be done in a GUI, while others can only be done in the command line.

*option* - see *flag*

*path* - A list of folders on your system that are checked for programs to generate the list of commands available on the command line. For example, since the folder `/bin` is typically on the path, putting an executable program in that folder will make it available as a command.

*pipeline* - in the command line, a pipeline is a sequence of processes. The output of one command feeds directly as input into the next command.

*prompt* - the `$` is known as the "prompt." It indicats that your command line is ready to receive commands.

*REPL* - "Read Eval Print Loop" The process of typing something in to the command line and getting something back out. Like most things to do with the command line, not as complicated (or scary) as it sounds.

*root* - A word for the administrative user on a system. You often need administrative privileges to install programs or access certain system folders using the command line. You can tell you're root when your `$` prompt turns into a `#` prompt. To become root, type `su` and enter the password you use to log in. (No characters or asterisks will appear, just type your password and press enter.) You can also run a single command as root by typing `sudo` before the command.

*Text editor* - A program for creating and editing plain text files. Unlike word processors such as LibreOffice and Word, which create complex documents in the form of archives that include formatting information and other metadata, a plain text editor creates a single file. Programmers tend to use plain text files because computers can work with them easily. Sublime Text, Nano, and VI are examples of text editors.

*UNIX* - A family of operating systems that have a multi-user model and a particular design philosophy. Both OSX and Linux are UNIXes. Windows is not.

*wildcard* `*` - the wildcard character on the command line will revolutionize your world. When you are giving a command an argument, for instance instead of

````grep filename.txt````

type

````grep *.txt````

The wildcard, `*`, will tell the command to search for any file ending with a .txt extension. But the wildcard can work anywhere in the string! If, for example, you want to move all formats (.doc, .pdf, .jpg) of the same name to a different folder you would type:

````mv [filename.*] [foldername]````


Find so much more on the command line:

[Bash manual](https://www.gnu.org/software/bash/manual/bashref.html) - the no nonsense text descriptions of bash commands.  
[explain shell](https://explainshell.com/) - a site that explains commands you paste into the form. This site is fantastic for breaking down commands you find in the wild on the internet.  
[Easy shell guide](https://lucasviola.github.io/easyshell/) - a friendly, styled (pastel!) list of common commands you might want to try out.
