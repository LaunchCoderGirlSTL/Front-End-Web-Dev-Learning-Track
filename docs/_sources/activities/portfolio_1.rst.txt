.. _portfolio_part1:

Portfolio - Part 1
==================

Setting Up Your Portfolio Project
---------------------------------

Intro
^^^^^

Yeah! First Project! Time to start writing some code!

You are going to start your Programmer Portfolio. This is what programmers typically use for their "resumes". It will hold links to all future projects as well as information about you!

We will start developing it here in the Learning Track but the real work on it will be done in the Project Track. For now, we are using it to practice writing code.

BUT FIRST!!

We need to setup our file structure, create some shell html css code and link your files.

Goals
^^^^^

1. To create and link your first html css files
2. To practice with the command line
3. To prep for your next assignments

Challenge Prep
^^^^^^^^^^^^^^

**STEP 1: Install Atom Command Line Tools**

For Mac Users:

1. Click *Atom > Install Shell Commands*
2. Open Terminal and test with the ``which atom`` command

.. image:: /_static/images/atom_install_mac.png
  :alt: Install Shell Commands Menu Option
  :width: 50%

For Windows Users:

1. Open Command Palette (``Cmd + Shift + P``)
2. Type "Window: Install Shell Commands"
3. Open Terminal and test with ``which atom``

.. image:: /_static/images/atom_install_windows.png
  :alt: Install Shell Commands Menu Option
  :width: 80%

**STEP 2: Watch a Brief Atom Text Edit Demo**

*This will be done in class.*

Challenge 1: Create your HTML and CSS file
##########################################

For this challenge you are going to use your command line. Remember these commands? 

::

  cd <path>
  mkdir <folder-name>
  touch <file-name>


Good! because today we are going to use them!

We are going to create the below file structure. 

::

  CoderGirl/
      portfolio_project/
          images/
              (empty for now)

          index.html
          main.css

**STEP 1**

Open your terminal. Make sure you are in your home directory (ie. ``Users/<user-name>``). We are going to create a folder (aka directory) here to keep all your CoderGirl Projects.

**STEP 2**

Use your command line and the ``mkdir`` command to create a new directory for your projects (I would probably call it "Projects" or "CoderGirl" but whatever works for you!).

.. note:: Remember when naming directories or files it is best to not use spaces because they look weird in path names.

**STEP 3**  

Now move *into* that new directory that you just created with the `cd` command. Create a new directory *here* for your just the code to your portfolio project. Recommend Name: "portfolio_project"

**STEP 4**  

Now move *into* that project directory with the ``cd`` command. so now if you do a ``pwd`` the file path printed below should look something like this but with the file names you used:  

``Users/<username>/CoderGirl/portfolio_project``

**STEP 5**  

Create File Structure (all within your terminal).

Use the ``touch`` command to create the following files:

* ``index.html``
* ``main.css``

Then create one more directory with the ``mkdir`` command named ``images``.

Your file structure should now look like this: 

:: 

  CoderGirl/
      portfolio_project/
          images/
              (empty for now)

          index.html
          main.css

**STEP 6**

Open your project directory with Atom.

Since we install the command line tools already, we can open our project with atom from the command line! yeah!

To do that we are going to use the atom command:

::

  atom <path-to-thing-you-want-to-open>


If I'm in the project directory (like if my ``pwd`` command prints something like this ``Users/<username>/CoderGirl/portfolio_project``)
then I can use the command ``atom .``, where the dot indicates I want to open the directory I am in.

If I was in the CoderGirl directory I would use the command ``atom portfolio_project`` to open the project directory.

Make sense? If you're confused ask a mentor :)

**STEP 7**

Copy and paste your starting HTML and CSS.  

.. note:: This is common practice in web development, starting with some HTML shell code.

.. code-block:: html

  <!DOCTYPE html>
  <html>
    <head>
      <title>Your Name</title>
      <link rel="stylesheet" type="text/css" href="styles/main.css">
      <meta content="width=device-width,maximum-scale=1.0,initial-scale=1.0,minimum-scale=1.0,user-scalable=yes" name="viewport">
    </head>

    <body>
      <div class='header'>
        <h1>Your Name</h1>
        <h2>Your Tagline</h2>
      </div>

      <div class='content'>
        <img src="images/thumbnail.png" alt="Your Github Username" class="thumbnail">
        <p>
          Who are you? What are you interested in? What are you doing to learn to code?
        </p>
      </div>
    </body>
  </html>


.. code-block:: css

  body {
    background-color: #eeeeee;
    color: #030303;
    margin: 0;
    padding: 0;
  }

  .header {
    padding: 15px;
  }

  .content {
    background-color: #030303;
    color: #eeeeee;
    padding: 15px;
  }

  p {
    margin: 0 15px;
  }

Challenge 2: Update the HTML
#################################

**STEP 1** Update All Text, including your name, tagline and a little description of yourself.

**STEP 2** Replace the Thumbnail Picture, with a picture of yourself.

**STEP 3** Change the colors of the site to match your preferences :)

That’s it for now! You will be coming back to this project to keep practicing what you have been learning.
