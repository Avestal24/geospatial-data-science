# Geospatial Data Science #

This repository contains course materials for GEOG490. The lecture notes are in the form of interactive [Jupyter Notebooks](https://jupyter-notebook.readthedocs.io/en/stable/examples/Notebook/What%20is%20the%20Jupyter%20Notebook.html).

## View the lecture notes online ##

The links below will render the notebooks via the [nbviewer](http://nbviewer.jupyter.org/) service, which allows some of the fancy interactive graphics to be viewed online. If you browse directly to the notebooks on github, they may not show up properly. So please use these links.

### Foundations
* 1: Course Overview
* 2: Version Control
* 3: Exploratory Data Analysis
* 4: Intro to Machine Learning

### Development
* Something
* Something else

## Run the lecture notes interactively ##

The best way to get the materials (including homework) is the use [git](https://git-scm.com/) to [clone this repository](https://git-scm.com/book/en/v2/Git-Basics-Getting-a-Git-Repository). If you don't have git already on you computer, it is easy to install on all platforms following [these instructions](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git).

From the command line, run the command

```bash
git clone https://github.com/JohnnyRyan1/geospatial_data_science
```

If you are not a fan of the command line, there are plent of [graphical interfaces to git](https://git-scm.com/download/gui/linux) available.

Once you have the repository cloned, you can update it as new lectures come out by running

```bash
git pull origin master
```

If for some reason you can't get git working, the alternative is to use the link to the right to "Download Zip". The disadvantage here is that you will have to re-download every time the repo is updated.

In order to actually execute the code in the notebooks, you need to have the necessary python packages installed.
The recommended way to do this is to install the [anaconda python distribution](https://www.anaconda.com/download/) together with the [conda package management utility](https://conda.io/docs/).
For more depth, you can read my [detailed intstructions for installing python](https://rabernat.github.io/research_computing/python.html).

This repository includes an [environment file](https://github.com/JohnnyRyan1/geospatial_data_science/blob/environment.yml) which you can use to set up your python environment. To install this environment, type the following

```bash
cd geospatial_data_science
conda env create -f environment.yml
```

This will create a new environment called `geospatial_data_science`. To activate this environment, type

```bash
source activate geospatial_data_science
```

The notebooks can be viewed and run using the [jupyter notebook](https://jupyter-notebook.readthedocs.io/en/stable/notebook.html) application. To launch the notebook interface, just type

```bash
jupyter notebook
```

When you are done working with the notebooks, close the notebook app and, if you wish, deactive the environment by typing

```bash
source deactivate
```

## Useful resources ##

* https://automating-gis-processes.github.io/site/course-info/course-info.html

## Why Python ##

A great deal has been written on [this subject](http://cyrille.rossant.net/why-using-python-for-scientific-computing/).
My reasons are summarized as follows.

1. __Python is open source__. [Open source](https://en.wikipedia.org/wiki/Open_source)
means that the source code is available freely to the public and can be examined,
modified, and improved. The alternative to open source is closed, proprietary.
Proprietary tools, such as MATLAB, are ultimately controlled by corporations, and
those corporations decide what features they will include. I consider software
tools as a central part of scientific research---if we want to have transparent,
reproducible, scientific results, we should be using open source tools.
[Nature](http://www.nature.com/nature/journal/v482/n7386/full/nature10836.html)
agrees with me.

1. __Python is free__. It does not cost money to use python. If your scientific
code is written in MATLAB, it can only be run by others with access to MATLAB.
That means people outside the university world (e.g. high school students), in
economically disadvantaged communities, or in developing countries will be
unable to reproduce and build on your results.

1. __Python is easy to read__. This may seem like a superficial point, but it is
crucial for effective sharing of code. Even if you are the only one reading
your code, python is easy on the eyes.

1. __Python has a great library__. The [scipy ecosystem](http://scipy.org)
provides the tools to do almost anything you can imagine.

1. __Python is constantly evolving__. If you find something you _can't_ do with
python, chances are someone is working on it. The world is changing: data is
exploding, computers architecture is evolving, and new forms of analysis and
visualization are being invented. Python is evolving too, and it evolves based
on what the community needs.

1. __Python is at home on the web__. The [Jupyter project](https://jupyter.org/)
grew out of the python community and is revolutionizing the way we do science
and communicate it with others. With Jupyter, I never have to leave my browser.
[Nature agrees](http://www.nature.com/news/interactive-notebooks-sharing-the-code-1.16261)
that this is the future of scientific communication.
