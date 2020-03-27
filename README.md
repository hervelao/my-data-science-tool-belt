# my-data-science-tool-belt
**NOTICE:** This repository may help students better navigate in the Machine Learning seas 🌊!

In the near future, I also intend to add a collection of minimal and clean implementations of machine learning algorithms (so that people would be able to easily play with the libraries), and add resources to help people better review their data science knowledge and prepare them for data science questions.

To install some of my packages, you can use pip:
```dash
pip install -r requirements.txt
```

Don't hesitate to contribute to the repo 🔥🔥🔥

## Summary

- [The Zen of Python](#the-zen-of-python) 🐍
- [Keyboard's shortcuts (Mac)](#keyboards-shortcuts-mac) 👩‍💻
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
- [Mastering Pandas](#mastering-pandas) 🐼
- [Mastering Data Visualization](#mastering-data-visualization)
  - [METHOD 1: MATLAB style plotting](#method-1-matlab-style-plotting-doc)
  - [METHOD 2: Object Oriented Interface](#method-2-object-oriented-interface-doc)
  - [Matplotlib & Seaborn demonstration](#matplotlib-&-seaborn-demonstration)
  - [Plotly demonstration](#plotly-demonstration)
- [Prerequisite warmup](#prerequisite-warmup)
- [Interesting posts](#interesting-posts)
- [Useful resources](#useful-resources)
- [Going further](#going-further)

## The Zen of Python

Beautiful is better than ugly.\
Explicit is better than implicit.\
Simple is better than complex.\
Complex is better than complicated.\
Flat is better than nested.\
Sparse is better than dense.\
Readability counts.\
Special cases aren't special enough to break the rules.\
Although practicality beats purity.\
Errors should never pass silently.\
Unless explicitly silenced.\
In the face of ambiguity, refuse the temptation to guess.\
There should be one -- and preferably only one -- obvious way to do it.\
Although that way may not be obvious at first unless you're Dutch.\
Now is better than never.\
Although never is often better than *right* now.\
If the implementation is hard to explain, it's a bad idea.\
If the implementation is easy to explain, it may be a good idea.\
Namespaces are one honking great idea -- let's do more of those!

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
split view into two columns                # cmd + alt + 2
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
git:(master)                               git checkout -b some-new-branch-name

# Remove the commit from the master branch
git:(some-new-branch-name)                 git checkout master
git:(master)                               git reset HEAD~ --hard

git:(some-new-branch-name)                 git checkout some-new-branch-name
# Your commit lives in this branch now
```

## Mastering Pandas

#### [10 minutes to pandas](https://pandas.pydata.org/pandas-docs/stable/getting_started/10min.html)

#### [Pandas Cheat Sheet](https://github.com/pandas-dev/pandas/blob/master/doc/cheatsheet/Pandas_Cheat_Sheet.pdf)

Below a small demonstration of main Pandas methods

```python3
# For printed results in Jupyter notebooks
pd.set_option("display.precision", 2)
pd.set_option('display.max_columns', 100)
pd.set_option('display.max_rows', 100)

# Basic methods
df = pd.read_csv('../data/file.csv')
df.head()
df.shape()
df.columns()
df.info()
df.describe() # for non-numerical features, add include=['object', 'bool']
df['Age'].value_counts() # to calculate fractions, add normalize=True

# Data types: bool, int64, float64 or object
df['Height'] = df['Height'].astype('int64')

# Sorting
df.sort_values(by='Age', ascending=False)
df.sort_values(by=['Age', 'Height], ascending=[True, False])

# Indexing and retrieving data
df['Height'].mean()
df[df['Age'] == 25].mean()
df[(df['Age'] == 25) & (df['Height'] < 185)]['Total minutes played'].mean()
df.loc[0:4, 'Age':'City'] # indexing by name, 4 and 'City' are inclusive
df.iloc[0:4, 0:5] # indexing by number, 4 and 5 are inclusive
df[-1:] # last line of the dataframe

# Applying and mapping functions
df.apply(np.max)
df[df['City'].apply(lambda city: city[0] == 'P')].head() # cities starting with P
df['column_name'] = df['column_name'].map({old_value: new_value})
SAME AS
df['column_name'] = df.replace({'column_name': {old_value: new_value}})

# Grouping
df.groupby(['Team'])[columns_to_show].describe(percentiles=[])
SAME AS
df.groupby(['Team'])[columns_to_show].agg([np.mean, np.std, np.min, np.max])

# Summary tables
pd.crosstab(df['Team'], df['Height']) # may add normalize=True
df.pivot_table(['Age', 'Height'], ['Team'], aggfunc='mean')

# Transformations
df['X_total'] = df['X1'] + df['X2']
df['X_total'] = df.apply(lambda row: row.X1 + row.X2, axis=1)
df["Player_height_mean"] = df.groupby('Player_ID')["Height"].transform('mean')
df.drop(['X1', 'X2'], axis=1, inplace=True) # got rid of columns
df.drop([1, 2]).head() # got rid of rows
```

## Mastering Data Visualization

#### [Data to Viz](https://www.data-to-viz.com/)
Leads you to the most appropriate graph for your data. It links to the code to build it and lists common caveats you should avoid.

2 interfaces for plotting:
- MATLAB style plotting using pyplot (METHOD 1);
- Object Oriented Interface (METHOD 2).

### METHOD 1: MATLAB style plotting ([doc](https://matplotlib.org/3.1.1/api/_as_gen/matplotlib.pyplot.html#module-matplotlib.pyplot))
```python3
plt.figure(figsize=(12, 8))
plt.plot(x, y**2, c='black', lw=3, ls='--', label='quadratic')
plt.plot(x, y**3, c='pink', lw=3, ls='--', label='cubic')
plt.title('title 1')
plt.xlabel('axe x')
plt.ylabel('axe y')
plt.legend()
plt.show()
plt.savefig('my_fig.png') # vector pdf image might be interesting

# To divide the figure in a 2x1 grid
plt.subplot(2,1,1)
plt.plot(x, y, c='orange')
plt.subplot(2,1,2)
plt.plot(x, y, c='blue')
```

### METHOD 2: Object Oriented Interface ([doc](https://matplotlib.org/api/axes_api.html#axis-labels-title-and-legend))
```python3
# Get an empty figure, a fig object can contain one or more axes objects
fig = plt.figure()

# Get the axes instance at 1st location in 1x1 grid, one axes represents one plot inside fig
# fig.add_subplot(2,2,1) would generate a grid of 2x2 subplots and and get for 1st location
ax = fig.add_subplot(1,1,1)

# Generate the plot
ax.plot(x, y)

# Set labels for x and y axis
ax.set_xlabel('X label')
ax.set_ylabel('Y label')

# Set title for the plot
ax.set_title('Title')

# Display the figure
plt.show()

# Another way to do it could be: fig, ax = plt.subplots(2, 1, sharex=True)
```

### Matplotlib & Seaborn Demonstration

Below a small demonstration of the main graphics and tables that can be used with matplotlib and seaborn ([example gallery using seaborn](https://seaborn.pydata.org/index.html))

```python3
# Import visualization libraries
import matplotlib.pyplot as plt
import seaborn as sns; sns.set()

# Change the display settings
%config InlineBackend.figure_format = 'retina' # Graphics are more sharp. 'svg'/'png'
plt.rcParams['figure.figsize'] = 8, 5
plt.rcParams['image.cmap'] = 'viridis'

# Histograms and density plots
df[features].hist(figsize=(10, 4));
df[features].plot(kind='density', subplots=True, layout=(1, 2),
                sharex=False, figsize=(10, 4)); # see 'kind='bar', or 'kde', 'scatter', etc
sns.distplot(df['feature']);

# Box plot
sns.boxplot(x='num_feature', y='cat_feature', data=df, orient='h');

# Violin plot
_, axes = plt.subplots(1, 2, sharey=True, figsize=(6, 4))
sns.boxplot(data=df['feature'], ax=axes[0]);
sns.violinplot(data=df['feature'], ax=axes[1]);

# Bar plot
_, axes = plt.subplots(nrows=1, ncols=2, figsize=(12, 4))
sns.countplot(x='cat_feat_1', data=df, ax=axes[0]); # can add "hue" for another cat_feat
sns.countplot(x='cat_feat_2', data=df, ax=axes[1]);

# Correlation matrix
corr_matrix = df[num_features].corr()
sns.heatmap(corr_matrix, annot=True, fmt=".1f", linewidths=.5);
# heatmap allows to view the distribution of a num over two cat

# Scatter plot and Scatter plot matrix
plt.scatter(df['X1'], df['X2']);
sns.jointplot(x='X1', y='X2', data=df, kind='scatter');
sns.jointplot('X1', 'X2', data=df, kind="kde", color="g");
sns.pairplot(df[numerical]);

# Plot with categories
sns.lmplot('X1', 'X2', data=df, hue='cat_feat', fit_reg=False);
fig, axes = plt.subplots(nrows=3, ncols=4, figsize=(10, 7))
for idx, feat in enumerate(numerical):
    ax = axes[int(idx / 4), idx % 4]
    sns.boxplot(x='cat', y=feat, data=df, ax=ax)
    ax.set_xlabel('')
    ax.set_ylabel(feat)
fig.tight_layout();
_, axes = plt.subplots(1, 2, sharey=True, figsize=(10, 4))
sns.boxplot(x='cat_feat', y='num_feat', data=df, ax=axes[0]);
sns.violinplot(x='cat_feat', y='num_feat', data=df, ax=axes[1]);
sns.catplot(x='cat_feat_1', y='num_feat', col='cat_feat_2',
               data=df[df['cat_feat_2'] < 3], kind="box",
               col_wrap=4, height=3, aspect=.8);
```

### Plotly Demonstration

The plotly library can also be used, that allows creation of interactive plots within a Jupyter notebook without having to use Javascript ([doc](https://plot.ly/python/))

```python3
from plotly.offline import download_plotlyjs, init_notebook_mode, plot, iplot
import plotly
import plotly.graph_objs as go

init_notebook_mode(connected=True)

# For line plots
trace0 = go.Scatter(  # Create a line (trace) for the GDP in France
    x=df.index,
    y=df['France GDP'],
    name='France GDP'
)

trace1 = go.Scatter( # Create a line (trace) for the GDP in Germany
    x=df.index,
    y=df['Germany GDP'],
    name='Germany GDP'
) # To use bar chart, you could've replaced 'go.Scatter' by 'go.Bar' in both

data = [trace0, trace1] # Define the data array
layout = {'title': 'France vs Germany GDPs'} # Set the title

fig = go.Figure(data=data, layout=layout) # Create a Figure and plot it
iplot(fig, show_link=False) # Visualize

plotly.offline.plot(fig, filename='gdp_stats.html', show_link=False); # Save the plot in an html file

# For box plots
data = []
for country in df.Country.unique():
    data.append(
        go.Box(y=df[df.Country == country].height, name=country)
    )
iplot(data, show_link=False) # Visualize
```

## Prerequisite warmup

####  Kaggle Learn, DataQuest [[Part1](https://www.dataquest.io/course/python-for-data-science-fundamentals/)/[Part2](https://www.dataquest.io/course/python-for-data-science-intermediate/)/[Part3](https://www.dataquest.io/course/pandas-fundamentals/)], CodeAcademy
Learn the basics of programming languages (Python, SQL)

#### [Essential Math for Data Science](https://hadrienj.github.io/), by Hadrien Jean
Basics of calculus, linear algebra, optimization and statistics are essential to understand the toolset you’re going to use. (Disclosure: I know the guy, and he's gold.)

#### 3blue1brown ([Essence of linear algebra](https://www.youtube.com/playlist?list=PLZHQObOWTQDPD3MizzM2xVFitgF8hE_ab)/[Essence of calculus](https://www.youtube.com/playlist?list=PLZHQObOWTQDMsr9K-rj53DwVRMYO3t5Yr)/[Neural Networks](https://www.youtube.com/playlist?list=PLZHQObOWTQDNU6R1_67000Dx_ZCJB-3pi)),  by Grant Sanderson
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
