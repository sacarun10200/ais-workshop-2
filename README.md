# AI Society Workshop - SciKit Learn
This is the GitHub repository for the Introduction to Machine Learning using SciKit-Learn and Python at UT Dallas. Install the following module dependencies to run the provided code in the Jupyter notebook.

* Numpy         (Math)
* Pandas        (Math)
* SciKit-Learn  (ML & Regression)
* Matplotlib    (Data visualization)

The easiest way to get this done is by installing Anaconda for Python, which helps with package management and comes pre-built with a lot of the packages required for Machine Learning. The appropriate install for your operating system can be found and downloaded here:\
https://www.anaconda.com/distribution/

Make sure the Anaconda package is properly added to your path by opening a terminal and running

`conda` 

The output should look like following. In this case, you can continue on to installing the packages, done below.

```
usage: conda [-h] [-V] command ...

conda is a tool for managing and deploying applications, environments and packages.
...
```

## Windows Troubleshooting
If it looks like the following, then Anaconda was not properly added to your PATH variable.
```
'conda' is not recognized as an internal or external command,
operable program or batch file.
```
You can find your PATH variables by doing the following.
```
Edit the system enviroment variables >
Environment Variables >
User variables for $USER >
Double Click Path
```
Let `$Anaconda` be the base install for the Anaconda package.

Add the following subfolders to your path\
`$Anaconda`\
`$Anaconda\Library\mingw-w64\bin`
`$Anaconda\Library\usr\bin`\
`$Anaconda\Library\bin`\
`$Anaconda\Library\Scripts`

For reference, my Anaconda base package was at 
`C:\Users\$USER\Anaconda3`

Exit out of the terminal and open a new one. `conda` should now be recognized.

## Package Install
If `conda` was correctly installed, we can now use `conda install $LibraryName` to install new packages, similar to `pip install`.

The packages above can be installed by
* `conda install numpy`
* `conda install pandas`
* `conda install sklearn`
* `conda install matplotlib`

---

## Material Covered
### Data Cleaning
* Data loading, cleaning, & labeling using SkLearn's `OneHotEncoder`
---
### Model Training
* K-Nearest Neighbors
* Decision Trees
* Logistic Regression