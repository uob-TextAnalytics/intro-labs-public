# intro-labs-public
Lab notebooks for Introduction to Text Analytics. Lab sheets will be added once the lab sessions have taken place.

## Setting up your environment

We recommend using ```conda``` to create an environment with the correct versions of all the packages you need for these labs. You can install either Anaconda or Miniconda, which will include the ```conda``` program. 

We provide a .yml file that lists all the packages you will need, and the versions that we have tested the labs with. You can use this file to create your environment as follows.

1. Open a terminal. Use the command line to navigate to the directory containing this notebook and the file ```crossplatform_environment.yml```. You can use the command ```cd``` to change directory on the command line.

1. Run the conda program by typing ```conda env create -f crossplatform_environment.yml```, then answer any questions that appear on the command line.

1. Activate the environment by running the command ```conda activate data_analytics```.

1. Make kernel available in Jupyter: ```python -m ipykernel install --user --name=data_analytics```.

1. Relaunch Jupyter: shutdown any running instances, and then type ```jupyter lab``` or ```jupyter notebook``` into your command line, depending on whether you prefer the full Jupyter lab development environment, or the simpler Jupyter notebook.

1. Find this notebook and open it up again.

1. Go to the top menu and change the kernel: click on 'Kernel'--> 'Change kernel' --> data_analytics.

You should now be ready to go!

The core libraries we will be using in this unit are:

- [Datasets](https://huggingface.co/docs/datasets/), produced by HuggingFace, is a hub for lots of interesting text datasets.
- [NLTK](https://www.nltk.org), a comprehensive NLP library.
- [Scikit-learn](https://scikit-learn.org/stable/user_guide.html), for machine learning and classifier evaluation.
- [Gensim](https://radimrehurek.com/gensim/), for topic modelling.

The libraries above have good documentation, which is available either online (links above) or via Python itself, e.g. `help(numpy.array)` in the Python interpreter. 

### Refreshers for Python and Jupyter

**Skip this part if you're already familiar with Python and Jupyter notebooks.**

This lab assumes you have used Python and Jupyter Notebooks before. 

For an introduction or refresher on Python, see the [Introduction to Python lab](https://github.com/UoB-COMS21202/lab_sheets_public/tree/master/lab_1) or the University of Bristol [Beginning Python](https://milliams.gitlab.io/beginning_python/) course. If you are a beginner with Python, you might also like to look at Chapter 1 in the NLTK book, which also provides a guide for "getting started with Python": https://www.nltk.org/book/ 

You will need to use Python 3, not Python 2, and Python 3.6 or newer are recommended.

The labs will be run on [Jupyter Notebook](http://jupyter.org/), an interactive coding environment embedded in a webpage supporting various programing languages (Python, R, Lua, etc.) through the concept of kernels.  

It allows you to enrich your code with complex comments formatted in Markdown and $\LaTeX$, as well as to place the results of your computation right below your code.

Notebooks are organised in cells which can contain either code (in our case, this will be Python code) or text, which can be easily and nicely formatted using the Markdown notation. 

To edit an already existing cell simply double-click on it. You can use the toolbar to insert new cells, edit and delete them (or use keyboard shortcuts which are very handy to speed up coding). 

Cells can be run, by hitting `shift+enter` when editing a cell or by clicking on the `Run` button at the top. Running a Markdown cell will simply display the formatted text, while running a code cell will execute the commands executed in it. 

**Note**: when you run a code cell, all the created variables, implemented functions and imported libraries will be then available to every other code cell. However, it is commonly assumed that cells will be run sequentially in terms of prerequisites. To reset all variables and functions (for debugging) simply click `Kernel > Restart` from the Jupyter menu.
