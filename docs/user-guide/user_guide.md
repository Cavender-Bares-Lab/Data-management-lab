# User guide

### Why this webpage?

Created, remove, and update documentation is essential for any
organization. This webpage was created for this aim using
[Mkdocs](https://www.mkdocs.org/) to satisfy the documentation
requirements for the lab.

This webpage does not not replaceable data storage requirements (e.g.,
group/cavender, google drive, or local drives). However, it allows users
to respond questions like:

-   Where is the data?
-   How the data was collected?
-   What protocol I need to be follow?
-   I am new here, what I need to do?
-   Among many others …

If you need to create, remove, or update documentation please follow the
bellows guide, or ask to the lab-technician for help.

<br>

### How to build this webpage?

To build this webpage, users must install on their computer:

-   [RStudio](https://www.rstudio.com/products/rstudio/download/) and
    [R](https://www.r-project.org/).
-   Rmarkdown and Knitr packages (e.g, `install.packages(rmarkdown)`).
-   [pip](https://pip.pypa.io/en/stable/cli/pip_install/)
-   [MkDocs](https://www.mkdocs.org/) (e.g., in terminal
    `pip install mkdocs`)
-   MkDocs material theme (e.i., in terminal
    `pip install mkdocs-material`)
-   [git](https://git-scm.com/downloads) and Github account.

<br>

#### Step 1 - Clone or update the webpage repository in your local machine.

If you and someone has been working on this webpage or you recent
started it is crucial to have the updated version.

If you recent started, you can clone the github repository to your local
machine using RStudio following:

    File > New Project ... > Select Version Control > Select Git 

You will see a ‘clone git repository’ window, add there the following
URL `https://github.com/Cavender-Bares-Lab/Data-management-lab.git` and
chose the project path of your preference.

In case you have been working on this webpage using RStudio interface,
it is a good practice to check if you have an updated version. For doing
so, you only need to click on the `Git` panel and then click on `pull`.
Remember that you will need git credentials.

This first step requires basic git skills, if you are a bit lost take a
look at this
[guide](https://www.geo.uzh.ch/microsite/reproducible_research/post/rr-rstudio-git/).

<br>

#### Step 2 - Let’s get familiar with Mkdocs.

In non-technical words, this webpage is composted by two elements: the
structure and the documentation.

-   The structure refers to the online appearance of the documentation,
    and it is controlled by `mkdocs.yml` file. In this file, under
    `nav:` you will see the structure of how the documentation and web
    sections will be displayed; their sections, tabs, and sub-tabs.

-   The documentation refers to the `.md` files located in the docs
    folder. These files contains all the information required that will
    be displayed in the webpage. It is a good practice to keep these
    files in folders under docs with names relatives to tabs and
    sub-tabs, just to keep the webpage in order.

Now that we know this elements, let’s take a look at three functions of
`MkDocs` that we will need to use. In RStudio you can run this command
using the ‘Terminal’ (the tab next to ‘Console’ that we always use).

-   `mkdocs serve`: this command help us to create local address where
    we can see the changes in our documentation in real time. This
    address tend to be `http://127.0.0.1:8000/` and it can opened using
    your browser.

-   `mkdocs build`:

-   `mkdocs gh-deploy`:

<br>

#### Step 3 - Let’s create a documentation file.

<br>

#### Step 4 - Let’s include the documentation in the .yml structure.

<br>

#### Step 5 - Let’s build the webpage, we are almost done!

<br>

#### Step 6 - Let’s publish the webpage!

<br>

#### Step 7 - Double check, we are done!

<br>

#### More questions?

For more instructions regarding how to build this page you could follow
this
[blog](https://ronnyhdez.github.io/blog/posts/2021-12-11-usingmkdocsrmd/).
Likewise, if you have questions regarding Mkdocs take a look at their
[webpage](https://www.mkdocs.org/).
