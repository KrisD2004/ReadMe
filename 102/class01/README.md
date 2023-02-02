# Markdowns paragraphs are like this(look at line 9-11)

Ex.I really like using Markdown.

I think I'll use it to format all of my documents from now on.

To create paragraphs, use a blank line to separate one or more lines of text.

If a paragraph isnt in a list then dont indent paragraphs with spaces or tabs(EX 15-18 you do)

Don't put tabs or spaces in front of your paragraphs.

Keep lines left-aligned like this.

(Lines 21-24 you dont do this)
   This can result in unexpected formatting problems.

  Don't add tabs or spaces in front of paragraphs.
  
## MARKDOWN HEADINGS

Markdown applications don’t agree on how to handle a missing space between the number signs (#) and the heading name. For compatibility, always put a space between the number signs and the heading name.
EXAMPLE:
(#Here is my heading) is wrong
(# Here is my heading) is the right way

You should also put blank lines before and after a heading for compatibility.
EXAMPLE:
Try to put a blank line before...

## Heading

...and after a heading.

DOING BOLD TEXT
To bold text, add two asterisks or underscores before and after a word or phrase. To bold the middle of a word for emphasis, add two asterisks without spaces around the letters.
EXAMPLE: 3 different ways
I really love **bold texting**
i love **chicken**
love**is**bold

## Basic Syntax

CommonMark and a few other lightweight markup languages let you use a parenthesis ()) as a delimiter (e.g., 1) First item), but not all Markdown applications support this, so it isn’t a great option from a compatibility perspective. For compatibility, use periods only.

Unordered Lists
To create an unordered list, add dashes (-), asterisks (*), or plus signs (+) in front of line items. Indent one or more items to create a nested list.
Unordered List Best Practices
Markdown applications don’t agree on how to handle different delimiters in the same list. For compatibility, don’t mix and match delimiters in the same list — pick one and stick with it.
To add another element in a list while preserving the continuity of the list, indent the element four spaces or one tab, as shown in the following examples.

## Revisions and the cloud

To be able to collaborate on Git Projects you would have to interact with Remote Repositories of a project residing online.
All teams can use remote repositories to push info to and pull data from.

*Cloned Repositories*
For Cloned repositories, Git will automactically give the "origin" to the server from which you had cloned and had named "master" to your local branch

*Seeing your remotes*
By running the git remote command, you can view the short names, such as “origin,” of all specified remote handles.

By using git remote -v, you can view all the remote URLs next to their corresponding short names.

WHAT IS GIT?
*Snapshots*
Git is a DVCS that stores data in a file system made up of "snapshots"
Everytime you save a changed version of your project called -COMMMIT- Git creates a "snapshot" of the file and stores a reference to it but if the file hasnt changed, Git only stores a reference to the already stored identical version of it.

*Local Operations*
Git most of time relies on *local operations* because most necessary info can be found in local resources.

*Tracking changes*
Every single change applied to any file or directory is tracked by Git. And, as the gatekeeper, Git will always detect file corruption or loss of information in transit

## loss of Data

Git is set up to greatly minimize the possibility of irreversible damage to files, such as accidentally lost data. Git makes it extremely difficult for a snapshot of your file that is committed to be lost.

*Distributed Version Control*
A Distributed Version Control systems (DVCS) addresses the major vulnerability of the CVS: the server as a single point of failure.

*Centralized Version Control*
The need for collaboration within a developer team on a single file or set of files led to the advent of the Centralized Version Control System (CVCS). This system entails a single server storing all changes and file versions, which can be accessed by various clients

WORKFLOW
*local reop structure*
The local git repo has 3 parts

1. Working Directory: the actual files are there
2. Index-area used for staging
3. head- points to the most recent commit

*Saving Changes*
All files in a working copy of a project file are either in a tracked state or untracked state
Tracked files can be modified, unmodified, or staged
Untacked files werent in the last snapshot and dont currently reside im the staging aera

*The life stages of file status*
First- after youve edited a file, Git flags it as modified because of the changes you had made after the previous changes
sec-- you staged the modified file
thired--you commit staged changes

*check file status*
To determine the state of files, utilize the git status command
EX---- $ git status

## Things i want to know

How does using Git help me become a better software engineer?

Summary:
This topic basically explains how to use all the elements on Git. From how to download it on mulitple op systems.
IT shows you how to setup and Git Repo
THis topic talks about cloning and about when you clone a file you have all the versions from a project
This tells you about the 3 componets of a local repo structure and the life cyle of a file

## The Coders computer

Test editor is a piece of software that you download and install on
your computer, or you access online through your web browser, that
allows you to write and manage text, especially the text that you write
to build a web site. The text editor has to be one of the most
important tools you can use as an aspiring web developer

CHOOSING AN EDITOR
Most important features are code completion, syntax highlighting, lots of themes to prevent eye strain and the ability to choose from a healthy selection of
extensions available when you need them

Code completion allows you to start typing, and the code completion
feature will display possible suggestions based on what you originally
typed. This saves you time by providing a choice, rather than allowing
you to finish typing and possibly encounter typos

The next feature that you should look for in a text editor is a nice
series of themes. These themes will allow you to change the color of
the background of your text editor, the series of colors in your text,
and sometimes themes will affect other aspects of your text editing
software as well. Usually, web developers use a dark background and
brightly colored text. Dark theme is easier on the eyes.

## THINGS I WANT TO KNOW MORE ABPUT

DO all text editors have mostly the same qualities?
Are all text editiors able manage all coding languages?
Do lighter themes for editiors make a difference?
