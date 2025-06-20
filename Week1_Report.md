#BASH COMMANDS LEARNED AND PRACTICED


Understanding file system:
the file system organises computer files and directories into a tree structure.

TRAVERSING THROUGH DIRECTORIES
    Command ls:
    the command line looks at the directory you are in, and then “lists” all the files and directories inside of it.



    Command pwd(print working director):

    It outputs the working directory. Working directory is the name of the directory you are currently in.



Command cd(change directory): We can change the directory using cd

we can do multiple changes like directory_1/directory_2/directory_3 and so on

	to move 2 directories, we can move using “ cd ../..”

	to move 1 directories we can move using “cd …"

MAKING DIRECTORIES AND FILES

    Command mkdir(Make directory): used for making directories
    Command Touch: Used for making files inside the working directory



VIEWING AND CHANGING FILES….


    Different ways to view files:

    ls -l: orders files and directories by the time they were last modified.

    ls -a: lists all files including hidden files and directories

    ls -t: Lists all contents in long format

    ls -alt: list all contents, including hidden files and directories, in long format, ordered by the date and the time they were last modified.
    ![CSV Output](./screenshots/Screenshot\ 2025-06-20\ at\ 12.05.41 PM.png)
    EXAMPLE:
    ![alt text](image.png)

ACCESSING FILES:

	COMMAND cat: outputs the contents of a specified file.

	Command cp: copies files from one file to another. the file that is getting the info often has the extension .bak….(revise)

		*(wildcard): used to copy all the files in that directory and can move it to a different directory(can use absolute path if you are getting too confused)

	Command mv: can be used to move and rename files.

	Command rm: removes files and directories

		syntax for directories is : rm -r directory

REDIRECTION:

	“>”: Is moves the output from one file to the other file using “Cat”

	“>>”: Appends data to the preexisting data in that file.

NOTE: DATA CAN BE REDIRECTED

	“|”:  Takes the standard output of the command on the left and pipes it as the standard input on the right.(revise)

	“sort”: sorting data alphabetically

	“uniq”: weeds out the repetitions

	“grep ”:  Looks for words in a file

		grep -i: looks words but is case insensitive

		grep -R: Searches for files with the word in a directory and lines in the file.

		grep -RL: Searches for just files in the directory with the word(better if you mention in the absolute address on the syntax).

PERMISSIONS:

	Syntax : chmod [owner][group][others] filename

		the parameters 




7 means read + write + execute.

[def]: image-1.png

#GIT COMMANDS LEARNED
Intro to GIT:

Git Workflow:
Git project can be thought of as having three parts:
	1.A working Directory - creating, editing , deleting and organizing files
	2.A staging area - where you will list changes you make to the working directory
	3.A repository - Stores changes permanently
![alt text][def4]


Init: initalizing a git repository

Status: 
git status is used to check the status of the changes in the working directory.

IMPORTANT:
In order to start tracking the file, the file needs to be added to the staging area.

WE CAN DO SO BY : git add filename

DIFF:
we can check the differences between the working directory and the staging area with:{git diff filename}

COMMIT: A commit permanently stores changes from the staging area inside the repository.
![alt text][def7]
LOG: commits stored in the repository can be viewed with {git log}

HEAD: most recent commits 

Checkout HEAD: gets the most recent workspace.

git reset HEAD filename: removes the file from the working area.
![alt text][def5]


INTRO TO GITHUB:
![alt text][def6]

branches isolate each teammate’s work in order to avoid conflicts in each others works.

INTRO TO BRANCHING:
	git branch: tells you which branch you are on
	git branch branch_name: lets you add a different branch
	git branch -d branch_name: lets you delete a different branch
NOTE: the * lets you know which branch you are on
	git checkout: lets you switch to a different branch
	git merge: lets you merge the branch you want to to the master branch(Note: you have to be on the branch you are merging into)

![alt text][def3]	



GENERAL PROCESS for pushing code:
![alt text][def2]

#Exception Handling
Exception handling:
	three types of errors:
		compile error(syntax error)
		runtime error(eg: divided by zero)—>most difficult error to fix
		logical error(wrong code)
		
we can create an exception for the errors using “try” and except.

Note: The code exists the try block once it finds an error.

to understand the exact error that occurs, use: (in the except block btw): except Exception as e: and then print(e).
print specific exception blocks in the first and the generic one in the last.

![alt text][def8]
Raising error:

We can “raise an error” using raise

An example of Raise.
![alt text][def9]

#UNDERSTANDING AND IMPLEMENTING PYTHON LIBRARIES FOR DATA ANALYSIS:
![alt text][def12]
![alt text][def13]


#REPORT:
This week’s training gave me a solid foundation in Linux, Python, and Git — three essential tools for any developer or data engineer. I started by learning how to navigate the Ubuntu terminal, use commands like ls, cd, and chmod, and create and manage files through the command line. Understanding file permissions, especially using chmod 600, was initially confusing, but became clear after practicing different combinations and seeing their effects on access rights.

In the Python section, I created basic scripts including a CSV reader using the csv module. The list comprehension part and understanding default parameters gave me a deeper insight into how Python makes things concise and efficient. Running scripts, managing virtual environments, and working with CSV files felt empowering because it made me realize how data can be ingested and processed in real-world scenarios.

The Git portion was a new experience, and although branching and merging were initially intimidating, practicing it step-by-step made the flow clearer. I especially liked seeing the Git log and understanding how version control can organize and protect your codebase.

#CHALLENGES I FACED:
Challenges I Encountered:
Adapting to a professional 8-hour work environment
One of the biggest challenges was simply adjusting to working full-time hours in a structured setting. I’m not yet used to sitting and focusing for long stretches, so building the mental stamina to stay engaged and productive throughout an entire workday was a major personal learning experience.

Understanding the command prompt from scratch
Coming into this training, I had zero background in using the terminal or command line. It felt completely foreign at first, and I ended up spending my entire weekend just getting comfortable with basic commands. Eventually, through repetition and trial-and-error, it started to make sense.

Learning Python from the ground up
I had minimal prior exposure to Python, so I had to start from the basics — variables, syntax, and control structures — and then quickly move into applying libraries like csv and random. It was challenging but also rewarding to go from knowing almost nothing to building functional scripts in just a few days. Then worked on pandas library for a data frame and use matplotlib to plot a scatterplot. Also found the correlation through pandas.
![alt text][def10]
![alt text][def11]

Visualizing GitHub and how version control works
Git and GitHub were hard to grasp conceptually at first — the idea of staging, committing, branching, and merging felt abstract. What really helped was experimenting hands-on and also using ChatGPT to explain the ideas in simpler terms and walk me through the steps.

#THE PYTHON FILES IS IN THE REPO IN GITHUB under Hello.py and tr.py as extensions



[def2]: image-2.png
[def3]: image-3.png
[def4]: image-7.png

[def5]: image-5.png
[def6]: image-4.png
[def7]: image-6.png
[def8]: image-8.png
[def9]: image-9.png
[def10]: image-10.png
[def11]: image-11.png
[def12]: image-12.png
[def13]: image-13.png