# Python Course IMAU 2024

Welcome to the IMAU Python Course 2024. This is an introductory workshop series on python specifically for the Climate Physics master programme at the Institute for Marine and Atmospheric research Utrecht (IMAU), Utrecht University

## Purpose
The main goal of the workshop is to bring all of you up to the same level of python programming. The other goal is that there are many specificities in working with geo-scientific data, so we want to provide some tools to help you in your studies.

## Course outline

### Topics covered

There are four modules covering the following topics:

0. Basics of programming in python
    - How to use notebooks
    - Data types, lists, dictionaries, loops, conditionals, functions, basic unix commands, classes
1. Packages: numpy, matplotlib, and scipy
    - Arrays, indexing, slicing, matrix operations
    - Plotting data, contour plot, subplots, quiver plots
2. Loading data with pandas, xarray and NetCDF4
    - DataFrame, operations, advantages of pandas
    - Reading and writing NetCDF data
    - Advanced xarray operations
3. Geo-scientific data: cartopy and modelling
    - Plotting spatial data, map projections, xarray integration
    - Numerical modelling with python

If you are already familiar with python, you can probably skip the first two modules. Modules 3 and 4 focus on specifics of the field of goesciences, so these modules could prove useful for all students. I will make the workshop materials available in advance, so that you can decide whether there is anything new to you.

Module 0 is a take-home assignment that you can do at your own leisure. If you have no experience with python we recommend that you do the entire module. For everyone else, feel free to scroll through the module. There still might be something useful in there (on classes for example). If you have any questions about Module 0 or about python installation, you can ask them during the Module 1 session or you can send me an email (w.s.j.kroese@uu.nl).

During the workshop I will shortly introduce the content lecture-style, but most of the time is reserved for exercises and questions that may arise. I will sent one more email before the first workshop. The main communication will be through Blackboard.

### Schedule

There are 3 sessions on Friday from 13:15 to 15:00 in the same room as the ACCP practical.
I will be there from 13:00 for those who need help with their installations.

|              | Date  | Time          |
| ------------ | ----- | ------------- |
| **Module 0** |   -   |       -       |
| **Module 1** | 13-09 | 13:15 - 15:00 |
| **Module 2** | 20-09 | 13:15 - 15:00 |
| **Module 3** | 27-09 | 13:15 - 15:00 |


## Python/Jupyter installation instructions:

For both the workshop and almost all master courses, you will need to have Python installed on your pc. In the workshops we will work with Jupyter Notebooks. If you have not installed Python and Jupyter yet, please see `Installation of Anaconda and Jupyter Notebook.pdf` for installation instructions.

## Course evaluation

This course has *no* course evaluation because it is not an official course that gives you EC's, but if you have feedback, please send it me (w.s.j.kroese@uu.nl) so that we can improve the course next year.


## Resources
* [Python introduction from w3schools](https://www.w3schools.com/python/python_intro.asp) where you can run code in the browser.
* [Earth and Environmental Data Science](https://earth-env-data-science.github.io/intro) full semester course by Ryan Abernathey at Columbia University from which much content is copied
* [IMAU's Python for Lunch workshop series](https://github.com/UU-IMAU/Python-for-lunch-Notebooks) a collection of workshop materials on topics of interest from IMAU students and researchers

<!-- 



## Purpose
We noticed in the last years that the programming background of everyone varies with some having zero experience and others having quite a lot already.
In addition, there are common specificities in working with (geo-) scientific data which you could all discover by yourselves, but why reinvent the wheel!?

## Workshop structure
There are four workshops.
The first two cover the basics of programming in python and if you feel comfortable with simple programming and plotting you will probably know this already and won’t want to attend.
The second two workshops focus on packages specific to our field and best practices for computational research projects.
I would thus recommend that all of you at least look at the contents of the last two workshops.
Below there is a list of resources that are worth checking out.

We meet Mondays during the after lunch time slot.
I will be there from 13:00 for those who need help with their installations.
The official workshop time is 13:15-15:00.

This is the current course outline:
1. [14.9.20 13:15-15:00] basic programming in python: data types, lists, dictionaries, loops, conditionals, functions, basic unix commands
2. [21.9.20 13:15-15:00] common python packages and basic plotting: numpy, matplotlib, scipy
3. [28.9.20 13:15-15:00] working with geoscientic data: netcdf data format, pandas, xarray
4. [5.10.20 13:15-15:00] mapping with cartopy, open science, and best practices

I will use jupyter notebooks for teaching because they can combine high quality documentation, code and output. For you to participate in the workshops you need to have a way to execute them. Please install Anaconda/Miniconda before the first workshop (see instruction below)!

The workshops are held online in MS Teams.
You can join the team `Python for Climate Physics` with the code I shared by email.
I will shortly introduce the content lecture-style, but most of the time is reserved for exercises and questions that may arise.
This is the first time I teach online, so things may change and even more than in normal times, I would like your feedback!
I will make the workshop materials available in advance, also so that you can decide whether there is anything new to you.
I will sent one more email before the first workshop, the rest of the communication will be via Teams.


---
## Python/Jupyter installation instructions:

For coherence, I strongly recommend we all use a Python installation with the conda package manager.
You have two (equally valid) options:
1. Anaconda: https://docs.anaconda.com/anaconda/install/ or 
2. Miniconda:  https://docs.conda.io/en/latest/miniconda.html
(NB: If you are on Linux or MacOS, you have a system python, but it is a good idea to install a separate Python version. Changing/adding to the system Python can lead to silly errors that are annoying to fix.)

The difference between the conda distributions is that Anaconda includes many packages (including some you will never use) and consequently uses up quite some disk space. It features a graphical user interface (the ![Anaconda Navigator](https://docs.anaconda.com/anaconda/navigator/)). Miniconda, on the other hand, only includes the bare necessities and packages need to installed as they are needed, thus using a lot less disk space. 

Once you have installed one of the two condas, there are two ways to work with jupyter notebooks:
1. jupyter notebook app: the basic, but sufficient option
2. jupyter lab app: the more advanced option

With Anaconda you can choose either app from the Navigator.

With Miniconda you need to install jupyter first.
You can do this by running `conda install jupyter jupyterlab` and subsequently confirming.
Then you can type in the terminal `jupyter notebook` or `jupyter lab` to start either of the two apps.
Also see the documentation that is linked in the paragraph above.

### Managing packages

The strength of Python is its extensive ecosystem of packages. There are pre-installed system libraries, but most packages need to be installed explicitely by you. Common packages we use include `numpy` (for array calculations) and `matplotlib` (for plotting). There are (again) several ways you can install packages:
1. in the terminal type `conda install {package}`, you can install several at the same time `conda install {package1} {package2} {package3}`
2. if you have Anaconda, you can use the Anaconda Navigator to search for and install packages

You can list all the packages in the current environment by typing `conda list`.

Sometimes conda does not "know" a package. Often these packages can be installed using an alternative channel (list of packages). Many smaller scientific packages are on the conda-forge channel and you can install them with `conda install -c conda-forge {special_package}`

---
## Resources
* [Earth and Environmental Data Science](https://earth-env-data-science.github.io/intro) full semester course by Ryan Abernathey at Columbia University from which much content is copied
* [IMAU's Python for Lunch workshop series](https://github.com/UU-IMAU/Python-for-lunch-Notebooks) a collection of workshop materials on topics of interest from IMAU students and researchers
 -->