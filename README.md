# UConn NumPy tutorial development
## Prof. Ryan C. Cooper
### This is our own repository for testing git and GitHub

This semester we are developing Jupyter notebooks for the [NumPy
tutorials repository](https://github.com/numpy/numpy-tutorials.git). We
are going to use a few tools to build tutorials, share code, and review
code:

## Building tutorials

__Python, Jupyter, and the SciPy stack__: You can install Python and NumPy with the [miniconda
installer](https://docs.conda.io/en/latest/miniconda.html). Once its
installed, you can run use the conda terminal to install NumPy, Jupyter,
SciPy, and Matplotlib

`$ conda install numpy jupyterlab scipy matplotlib`

If you're new to NumPy, get started with the [Absolute Beginner's
Tutorial to NumPy](https://numpy.org/devdocs/user/absolute_beginners.html). 

In your conda terminal, run

`$ jupyter-lab`

to get Jupyter running in a web browser (I prefer Firefox or Chrome).
Now, you can run some Python commands and make some progress.

## Sharing code

__GitHub and Git__: NumPy is a free open source software. The code is
updated using a version control software called
[git](https://git-scm.com/downloads). NumPy is shared and reviewed by a
worldwide community of developers on the website <www.github.com>. You
can download, share, and suggest changes to software using git and
GitHub. Start by installing [git](https://git-scm.com/downloads), then
use a terminal to clone this repository

$ git clone https://github.com/cooperrc/uconn_numpy_tutorials

Once you have run this command, you now have a copy of this repository
on your computer. Try opening the practice_notebook.ipynb in the
notebooks folder and running the commands. You can play around with the
inputs and even write your own code. 

## Reviewing code

__GitHub Pull Requests__: We will get code reviewed by creating a pull
request (PR) on an existing GitHub repository. Practice creating a PR
with these steps:

1. Create a
[fork](https://docs.github.com/en/github/getting-started-with-github/fork-a-repo)
of the repository
[uconn_numpy_tutorials](https://github.com/cooperrc/uconn_numpy_tutorials)

2. Clone your fork to your computer with the `git clone ...`

3. Create a new "remote" for the upstream repo with the command

`git remote add upstream https://github.com/cooperrc/uconn_numpy_tutorials`

4. Use the `git` command to create a "branch" called my-notebook

`git branch my-notebook`

5. Use the `git` command to "checkout the branch"

`git checkout my-notebook`

6. Create your own Jupyter notebook in the notebooks folder, use your
username to make it unique e.g. I would name the notebook,
cooperrc_notebook.ipynb

  a. In your notebook include a NumPy example that you think is
  interesting
  
  b. Save your work and close the notebook

7. Use the `git` command to (i) add your file, (ii) commit your work,
and (iii) push your changes to your fork

  i. `git add notebooks/cooperrc_notebook.ipynb`
  ii. `git commit -m "my first branch commit for my notebook"`
  iii. `git push -u origin my-notebook`

8. Now, you can [create a
PR](https://docs.github.com/en/github/collaborating-with-issues-and-pull-requests/creating-a-pull-request#creating-the-pull-request)
with this repository and I will merge your work.  

__Bonus:__ [contributing to your first open source project](https://towardsdatascience.com/getting-started-with-git-and-github-6fcd0f2d4ac6)
