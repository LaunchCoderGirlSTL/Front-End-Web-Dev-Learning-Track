=================
My Portfolio Site
=================

-----
Setup
-----

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

----------
Git Going!
----------

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

----
HTML
----

Getting Started
---------------

Stub out index.html with these basic elements:

1. the HTML5 doctype
2. ``<html>``
3. ``<head>``
4. ``<title>``
5. ``<body>``

and fill each element with some appropriate content. You can start by removing the snippet of HTML that you added during setup.

Getting to Work
---------------

Your mission is to create a resume page that tells the story of your professional journey to-date, and where you want to go as a coder.

Here are the requirements:

1. Uses each of the following structural HTML5 tags: ``<p>``, ``<header>``, ``<footer>``, ``<main>``, ``<article>``. If you need to brush up on what each of these tags is used for, or if any of them are new to you, check out the `HTML tag reference <https://www.w3schools.com/tags/default.asp>`_ at w3schools.

2. Uses at least one HTML entity.

    .. hint:: 
       Putting a copyright notice in your footer will afford you the opportunity to use &copy;, but you should also try to get creative here.


3. Is creative. Don't stop with these items or tags. Have some ideas for your page, and make it great. And dig into the w3schools HTML reference to learn more about other tags, their usage and attributes!

Notes and Tips 
==============

Use your browser developer tools to look at the example page, or to troubleshoot things that don't look right. You can mimic the document structure of this example, but **do not just copy/paste**! Use the example to learn how your HTML elements might be structured, and structure your own page according to your own content's needs.
Don't add any CSS yet. Really, we mean it! If you think your page looks boring now, that's okay. We'll get there soon enough.
As you make changes, you will obviously want to see the results. To do so, simply re-save the file in your text editor, and then, over in your browser window, click Refresh (or use cmd+R on a Mac, ctrl+R on Windows).
Rely on reference sites linked on this page, and elsewhere online. We haven't taught you every detail about every tag that you may want or need to use, and you're free to use tags that haven't been explicitly introduced in class. We've given you enough background to get started, and are intentionally leaving some of the learning up to you.

Add and Commit Your Changes on Git
----------------------------------

Once you are finished, use Git once again to ``add`` and ``commit`` your index.html changes.

Why again?

The reason is that, since you have added a bunch of new HTML code, your index.html file is now in a very different state from how it looked the first time you committed it. You can see this by checking your status:

.. code-block:: bash

   $ git status
   On branch master
   Changes not staged for commit:
     (use "git add <file>..." to update what will be committed)
     (use "git checkout -- <file>..." to discard changes in working directory)

        modified:   index.html

   no changes added to commit (use "git add" and/or "git commit -a")

Git is telling us: `I see that you have modified` ``index.html``. `Use` ``git add`` `if you want this file's changes to be included in your next commit.`

At the risk of oversimplifying a bit, the Git workflow more or less comes down to this:

1. Create some initial stuff
2. ``init``
3. ``add`` and ``commit``
4. Make some changes
5. ``add`` and ``commit``
6. Make some more changes
7. ``add`` and ``commit``

and so on until the project is complete!

The general rule is that whenever you make any changes, you must add and commit those changes to Git.

So let's now go ahead and do that. From within your root ``my_portfolio_site``/ directory:

.. code-block:: bash

   $ git add index.html
   $ git commit -m "Finished work on HTML page"

You might be wondering: `How do I know when it's time to pause working and do another commit?`

This is somewhat subjective, and ultimately up to you. The basic guiding principle is that you should pause and commit any time you have reached a natural stopping point and completed a coherent "chunk of work".


