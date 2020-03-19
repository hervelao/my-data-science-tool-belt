# my-data-science-tool-belt
**NOTICE:** This repository is aimed to help students better understand Data Science.
Don't hesitate to contribute to the repo ;)

## Summary

- [The Zen of Python](#the-zen-of-python)🐍
<!-- - [A Parable by Sir Arthur Conan Doyle](#a-parable) -->
- [Keyboard's shortcuts (Mac)](#keyboards-shortcuts-mac)
  - [Sublime Text](#sublime-text)
  - [Terminal](#terminal)
  - [Chrome](#chrome)
  - [Jupyter Notebook](#jupyter-notebook)
  - [Jupyter Lab](#jupyter-lab)
  - [Magic functions](#magic-functions)
- [Mastering git](#mastering-git)
  - [How to use features branches](#how-to-use-features-branches)
  - [How to push a branch to GitHub](#how-to-push-a-branch-to-github)
  - [How to merge your branch to the master branch](#how-to-merge-your-branch-to-the-master-branch)
  - [How to solve your conflicts](#how-to-solve-your-conflicts)
  - [How to fix an accidental commit to master](#how-to-fix-an-accidental-commit-to-master)
- [Prerequisite warmup](#prerequisite-warmup)
- [Interesting posts](#interesting-posts)
- [Useful resources](#useful-resources)
- [Going further](#going-further)

## The Zen of Python

Beautiful is better than ugly.
Explicit is better than implicit.
Simple is better than complex.
Complex is better than complicated.
Flat is better than nested.
Sparse is better than dense.
Readability counts.
Special cases aren't special enough to break the rules.
Although practicality beats purity.
Errors should never pass silently.
Unless explicitly silenced.
In the face of ambiguity, refuse the temptation to guess.
There should be one -- and preferably only one -- obvious way to do it.
Although that way may not be obvious at first unless you're Dutch.
Now is better than never.
Although never is often better than *right* now.
If the implementation is hard to explain, it's a bad idea.
If the implementation is easy to explain, it may be a good idea.
Namespaces are one honking great idea -- let's do more of those!

<!-- ## A Parable

The cheese-mites asked how the cheese got there,\
And warmly debated the matter;\
The Orthodox said that it came from the air,\
And the Heretics said from the platter.\
They argued it long and they argued it strong,\
And I hear they are arguing now;\
But of all the choice spirits who lived in the cheese,\
Not one of them thought of a cow.

BY SIR ARTHUR CONAN DOYLE

Cast your eyes in the direction of the cow. 🐄 -->

<!-- <div align="center">

![cow](https://github.com/hervelao/my-data-science-tool-belt/blob/master/img/cow.jpg)

</div> -->

## Keyboard's shortcuts (Mac)

### Sublime Text
```python3
open a file in current project             # cmd + P (or cmd + T)
move a line upwards in file                # ctrl + cmd + ↑
move a line downwards in file              # ctrl + cmd + ↓
(un)comment lines                          # cmd + shift + / (or cmd + /)
search in file                             # cmd + F
search in project                          # cmd + shift + F
add package                                # cmd + shift + P
add indentation                            # tab
remove indentation                         # shift + tab
reach next word                            # alt + →
reach previous word                        # alt + ←
reach end of line                          # cmd + →
reach beginning of line                    # cmd + ←
close tab                                  # cmd + w
reopen last tab closed                     # cmd + shift + T
navigate to tab on the right               # cmd + alt + →
navigate to tab on the left                # cmd + alt + ←
duplicate line                             # cmd + shift + D
split view into two columns                # cmd + option + 2
(un)toggle sidebar                         # cmd + K, cmd + B
select similar words                       # cmd + shift + G
put cursor in several places               # cmd + click
```

### Terminal
```python3
open a new tab                             # cmd + T
close tab                                  # cmd + W
clear window (keeping history)             # ctrl + L
clear window (losing history)              # cmd + K
reach next word                            # alt + →
reach previous word                        # alt + ←
reach beginning of line                    # ctrl + A
reach end of line                          # ctrl + E
erase the whole line                       # ctrl + U
navigate to tab on the right               # cmd + shift + →
navigate to tab on the left                # cmd + shift + ←
```

### Chrome
```python3
open developer tools (elements)            # cmd + alt + I
open developer tools (console)             # cmd + alt + J
navigate to tab on the right               # cmd + alt + →
navigate to tab on the left                # cmd + alt + ←
open a new tab                             # cmd + t
open a new incognito window                # cmd + shift + N
Show downloads                             # cmd + shift + J
focus on address bar                       # cmd + L
close tab                                  # cmd + W
reopen last tab closed                     # cmd + shift + T
hard refresh (clear cache)                 # cmd + shift + R
```

### Jupyter Notebook
```python3
BOTH MODES:
run selected cell                          # ctrl + enter
run cell and insert below                  # alt + enter
run cell and select below                  # shift + enter
save and checkpoint                        # cmd + S

COMMAND MODE:
enter command mode (blue):                 # esc (or click anywhere outsite the cell)
add new cell above the current one         # A
add new cell below the current one         # B
delete selected cells                      # D, D (press the key twice)
open command palette                       # P
show all shortcuts                         # H
selected cells above                       # shift + ↑
selected cells below                       # shift + ↓
cut selected cells                         # X
copy selected cells                        # C
paste cells below                          # V
undo cell deletion                         # shift + V
change the cell type to Code               # Y
change the cell type to Markdown           # M
scroll notebook up                         # shift + space
scroll notebook down                       # space

EDIT MODE:
enter edit mode (green):                   # enter (or click in a cell)
(un)comment lines                          # cmd + ! (or cmd + /)
put cursor in several places               # cmd + click
open command palette                       # cmd + shift + P
indent                                     # tab
open tooltip                               # shift + tab
```

🚀 For more keyboard shortcuts, Help -> Keyboard Shortcuts from Menu bar.


♥️ nbextensions


`pip install jupyter_contrib_nbextensions` \
`pip install jupyter_nbextensions_configurator` \
`jupyter contrib nbextension install --user` \
`pip install rise`

### Jupyter Lab
```python3
BOTH MODES:
run selected cell                          # ctrl + enter
run cell and insert below                  # alt + enter
run cell and select below                  # shift + enter
save notebook                              # cmd + S
save notebook as                           # cmd + shift + S

COMMAND MODE:
enter command mode (blue):                 # esc (or click anywhere outsite the cell)
add new cell above the current one         # A
add new cell below the current one         # B
delete selected cells                      # D, D (press the key twice)
selected cells above                       # shift + ↑
selected cells below                       # shift + ↓
cut selected cells                         # X
copy selected cells                        # C
paste cells below                          # V
change the cell type to Code               # Y
change the cell type to Markdown           # M

EDIT MODE:
enter edit mode (green):                   # enter (or click in a cell)
(un)comment lines                          # cmd + ! (or cmd + /)
put cursor in several places               # cmd + click
indent                                     # tab
```

### Magic functions
```python3
compute time for your code to run          # %%time
show your plots (Jupyter Lab)              # %matplotlib inline

reload the kernel every time..             # %load_ext autoreload
..you change something in your code        # %autoreload 2

show the variables in your environment     # %who_ls
```

## Mastering git

2 master rules:
- Never commit directly to master. Use feature branches;
- Always make sure git status is clean pull, checkout or merge.

⚠️ Don't forget to sweep or delete your branches when they've become unnecessary!
`git branch -d branchname`

### How to use features branches

```dash
git:(master)                               git status
# Make sure it is clean

git:(master)                               git checkout -b my-new-feature
git:(my-feature)                           git branch
```

We've created a new local branch called my-new-feature.
Therefore, any new commit will only apply to this branch.

### How to push a branch to GitHub

```dash
git:(my-feature)                           git add .
git:(my-feature)                           git commit -m 'clear and meaningful commit'
git:(my-feature)                           git push origin my-feature

git:(my-feature)                           git status
# Make sure this is clean

git:(my-feature)                           hub browse
# You can now create a pull request on GitHub

git:(my-feature)                           git checkout master
git:(master)                               git pull origin master
git:(master)                               git sweep

git:(master)                               git checkout -b my-new-feature
```

### How to merge your branch to the master branch

```dash
git:(my-new-feature)                       git add .
git:(my-new-feature)                       git commit -m 'clear and meaningful commit'

git:(my-new-feature)                       git status
# Make sure this is clean

git:(my-new-feature)                       git checkout master
git:(master)                               git pull origin master

git:(master)                               git checkout my-new-feature
git:(my-new-feature)                       git merge master
```

### How to solve your conflicts

When you can't merge because of conflicts in an `unmergeable_branch`, follow this process:

```dash
git:(unmergeable_branch)                   git status
# Make sure this is clean

git:(unmergeable_branch)                   git checkout master

git:(master)                               git pull origin master

git:(unmergeable_branch)                   git checkout unmergeable_branch

git:(unmergeable_branch)                   git merge master

# Now you've fetched all conflicts locally, time to solve them 🕵️‍♀️
# Open your code editor and solve conflicts (locate them with cmd + shift + F)

# After that, you can commit your code
git:(unmergeable_branch)                   git add .
git:(unmergeable_branch)                   git commit -m "conflict solving"
git:(unmergeable_branch)                   git push origin unmergeable_branch

git:(unmergeable_branch)                   hub browse
# You can now create a pull request on GitHub

git:(unmergeable_branch)                   git checkout master
git:(master)                               git pull origin master
git:(master)                               git sweep

git:(master)                               git checkout -b my-new-feature
```

### How to fix an accidental commit to master

When you committed some changes to `master` and wanted to commit them to a new branch, follow this process:

```dash
# First, create a new branch from the current state of master
git:(master)               git checkout -b some-new-branch-name

# Remove the commit from the master branch
git:(some-new-branch-name) git checkout master
git:(master)               git reset HEAD~ --hard

git:(some-new-branch-name) git checkout some-new-branch-name
# Your commit lives in this branch now
```
## Prerequisite warmup

####  Kaggle Learn, DataQuest [[Part1](https://www.dataquest.io/course/python-for-data-science-fundamentals/)/[Part2](https://www.dataquest.io/course/python-for-data-science-intermediate/)/[Part3](https://www.dataquest.io/course/pandas-fundamentals/)], CodeAcademy
Learn the basics of programming languages (Python, SQL)

#### [Essential Math for Data Science](https://hadrienj.github.io/), by Hadrien Jean
Basics of calculus, linear algebra, optimization and statistics are essential to understand the toolset you’re going to use. (Disclosure: I know the guy, and he's gold.)

#### 3blue1brown ([Essence of linear algebra](https://www.youtube.com/playlist?list=PLZHQObOWTQDPD3MizzM2xVFitgF8hE_ab)/[Essence of calculus](https://www.youtube.com/playlist?list=PLZHQObOWTQDMsr9K-rj53DwVRMYO3t5Yr)/[Neural Networks](https://www.youtube.com/playlist?list=PLZHQObOWTQDNU6R1_67000Dx_ZCJB-3pi)),  by Grant Sanderson,
Some combination of math and entertainment. The goal is for explanations to be driven by animations and for difficult problems to be made simple with changes in perspective. BIG MVP!!!

#### [What REALLY is Data Science? Told by a Data Scientist](https://youtu.be/xC-c7E5PK0Y)
Spoilers: Solve real company problems using data.

## Interesting posts

#### [How It Feels to Learn Data Science in 2019](https://towardsdatascience.com/how-it-feels-to-learn-data-science-in-2019-6ee688498029)
Funny satire.

#### [The Unreasonable Effectiveness of Recurrent Neural Networks](http://karpathy.github.io/2015/05/21/rnn-effectiveness/)
Shows you the power of RNNs.

#### [XKCD](https://xkcd.com/) & [Saturday Morning Breakfast Cereal](https://www.smbc-comics.com/)
Webcomics of romance, sarcasm, science, and language by Randall Munroe and Zach Weinersmith.

## Useful resources

#### [Morning Brew](https://www.morningbrew.com/daily/r/?kid=450c54be) & [Emerging Tech Brew](https://www.morningbrew.com/emerging-tech/r/?kid=450c54be)
The daily email newsletter covering the latest news from Wall St. to Silicon Valley. Informative, witty, and everything you need to start your day.

#### [Data to Viz](https://www.data-to-viz.com/)
Leads you to the most appropriate graph for your data. It links to the code to build it and lists common caveats you should avoid.

#### [Projector Tensorflow](https://projector.tensorflow.org/)
Visualize data like you have never seen it before.

#### [LeetCode](https://leetcode.com/problemset/all/) & [CodeWars](https://www.codewars.com/users/sign_in)
Level up your coding skills, and achieve code mastery through challenge.

#### [Streamlit](https://www.streamlit.io/)
Quickly Build and Deploy a Dashboard.

#### [Google Data Studio](https://datastudio.google.com/u/0/navigation/reporting)
Unlock the power of your data with interactive dashboards.

## Going further

#### [Google Machine Learning Crash Course](https://developers.google.com/machine-learning/crash-course/ml-intro) & [Open Machine Learning Course mlcourse.ai](https://mlcourse.ai/)
Basic Machine Learning is covered here. Wonderfully well explained.

#### [Kaggle](https://www.kaggle.com/)
The world's largest data science community with powerful tools and resources to help you achieve your data science goals. Learn from all previous competitions 🙏
