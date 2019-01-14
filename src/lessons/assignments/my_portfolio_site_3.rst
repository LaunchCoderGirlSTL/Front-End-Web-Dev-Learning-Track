=========================
My Portfolio Site: Part 3
=========================

------------
Requirements
------------

1. Add Bootstrap to your site. 
2. Add screenshots of your site on multiple display sizes to the README of your site's Github repo.

-----------------
Before you start!
-----------------

In the next lesson, we will be talking about CSS layout tools, some of which will handle repsonsive design for you. So to get started, we are going to create a new branch in git so that we can add Bootstrap without it interfereing with our work for the next lesson.

To do so:

1. Type ``git status`` in your project directory. At the top of the output, you will notice the first line states: ``On branch master``.
   
   .. note::
      Branches in Git are like the branches of a tree. They are all tied to the same base, however, each one is unique and carries with it different attributes. Branches should be used when experimenting with new features. Once you are confident in the code in one branch, you can always merge that branch back into the master branch.

2. To create a new branch, type ``git checkout -b bootstrap`` and not only will a new branch be created, but you will also be switching your workflow over to a new branch. 

    .. hint::
       If you ever want to switch back to your master branch or any other branch in your project simply type ``git checkout branch-name`` with ``branch-name`` being the name of the branch you want to switch over to.

3. Now type ``git status``. The output should look like:

    .. code-block:: bash
       
       $ git status
       On branch bootstrap
       nothing to commit, working directory clean

4. Now you are ready to get started!

----------------
Adding Bootstrap
----------------

1. Your goal is to add Bootstrap to your portfolio site. Without messing up the layout you worked so hard on for your resume page, create a new HTML file called ``resume.html`` in your project directory. 

    .. hint::
       If you cannot remember how to do this, refer back to the assignment page from Lesson 3. 

2. Take the content you put in ``index.html`` and copy it over into ``resume.html``. We are doing this to create a landing page for your portfolio site. We want to keep the homepage minimal and link off of it.
3. Link ``resume.html`` on to your ``index.html`` page with an ``<a>`` tag.
4. Add other elements to your homepage, such as a link to your Github profile or your name in snazzy colors. Get creative here!
5. Add Bootstrap to the site.

------------------
After you are done
------------------

1. Use ``git status`` to confirm your changes, ``add``, and ``commit``. Remember when you ``push``, that the command will be ``git push origin bootstrap``!
2. Add a few screenshots of your site displayed on multiple different displays to your README. Your README serves as your documentation, so it is helpful to keep track of changes and the effect those changes had there whenever you are working on a project.