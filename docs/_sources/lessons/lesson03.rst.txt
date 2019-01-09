==============
Lesson 3: HTML
==============

Prep Work
---------

Complete Lesson 1: HTML Syntax from an `Intro to HTML and CSS <https://www.udacity.com/course/intro-to-html-and-css--ud001/>`_.

In-class Work
-------------

After going over the baics of HTML with your instructors, start working on your assignment. The directions are below. 

Assignment
----------

Your assignment is to start building your portfolio site. We will be covering different elements that will make this site look better over the coming weeks, so don't panic if it doesn't look the way you want it to today!

1. Navigate into the parent folder where you keep all your course materials (e.g. ``codergirl/`` or ``code/``). Only you know where that folder lives in your file system.

2. Make a new folder for this assignment with the  ``mkdir`` command. For example, ``mkdir my_portfolio_site``.

3. Within your new ``my_portfolio_site/ directory``, create and save a new file called ``index.html``:

    .. code-block:: bash

       $ touch index.html

    .. note::
           The filename ``index.html`` is a standard convention for the name of the root page of a website. Most web servers will treat ``index.html`` as the default file to load from a given directory.

4. Open up your new file in a text editor. Add a single line with the following HTML:

    .. code-block:: html

       <p>YOUR NAME</p>


5. Save your file.

6. Finally, open up the file in a web browser. You can do this by selecting File > Open File in your web browser, and navigating to the location of your new HTML file.

You should see a blank white page with your name in the top-left corner.

Git Going!
==========

Now let's incorporate Git into the picture.

1. **Initialize the project as a Git repository.** 
    In your terminal, make sure you are inside your ``my_portfolio_site`` folder, and then use the ``git init`` command to initialize that folder as a Git repository:

    .. code-block:: bash
    
       $ pwd
       /Users/adalovelace/codergirl/my_portfolio_site
       $ git init
       Initialized empty Git repository in /Users/adalovelace/codergirl/my_portfolio_site/.git/

    .. note::
           In place of adalovelace, put your name

    Now your project is a Git repository, which will enable you to use all of the magic Git powers:

    * using version-control to manage your changes
    * syncing your local repository with a remote repository on Github.com.

    .. note::
           You will only have to use the command ``git init`` once at the beginning of the project.
2. **Check your status**
    Back in the terminal, use the ``git status`` command to check the status of your newly created repo:

    .. code-block:: bash

       $ git status
       On branch master

       Initial commit

       Untracked files:
         (use "git add <file>..." to include in what will be committed)

               index.html

       nothing added to commit but untracked files present (use "git add" to track)

    This message says a lot of things, but for now, the most important point is that ``index.html`` is currently "untracked". We need to ``add`` and then ``commit`` the file so that Git can help us manage its changes.
3. **Add your work to the repo**
    Use the git add command to track your index.html file so that it will be staged for your next commit:

    .. code-block:: bash

       $ git add index.html

4. **Check your status**
    If you check your status again, you should see that your change (the creation of the new file) is staged to be committed:

    .. code-block:: bash

       $ git status
       On branch master

       Initial commit

       Changes to be committed:
         (use "git rm --cached <file>..." to unstage)

           new file:   index.html

5. **Commit**
    Now you are ready to ``commit`` the changes you have staged.
    Go ahead and commit your changes, along with an appropriate message describing what you have changed:

    .. code-block:: bash

       $ git commit -m "Created index.html file"

6. **Check your status**
    Now that you have committed, your status should be "clean":

    .. code-block:: bash

       $ git status
       On branch master
       nothing to commit, working directory clean



