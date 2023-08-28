# Pandas 🐼 and Git 🫴🏼 task
This task is fully customizable, you can choose to do it however may you like, but you have to do it. You are encouraged to use the internet to search for answers, use information from the task Menna sent you, and use info from this task there. And of course ask your colleagues for help whenever you need it! 🤗
## Pandas 🐼

### 1. What is Pandas?

Pandas is a Python library used for working with data sets, you should know this by now. It has functions for analyzing, cleaning, exploring, and manipulating data. The name "Pandas" has a reference to both "Panel Data", and "Python Data Analysis" and was created by Wes McKinney in 2008.

Speaking of *analyzing, cleaning, exploring, and manipulating* data, what functions can you use for each of these tasks? 🤔:
- **A**nalyze data?
- **C**lean data?
- **E**xplore data?
- **M**anipulate data?

**Fill the table below:**
  

function | what it does | category
------------ | ----------- | ---------
`astype()` |`converting types`| `C`  
`groupby()` |`convert a category column to be an index with its value`| `A`  
`sort_values()` |`sort the data by columns you put in parametar by`| `E`  
`pivot_table()` |`same as groupby but you have the ability to spcify the rows and columns`| `A`  
`merge()` |`merging to data sets with each other`| `M`  
`plot()` |`drowing the data`| `E`  
`corr()` |`finding the pairwise correlation of all columns in the data`| `E`  
`cov()` |`finding the covariance of each column`|`E`  
`apply()` |`appling function to every column or in every value in a column`|`M` `E`  
`loc()` |`show a row in the data but with a label string not a number`|`E`  
`iloc()` |`show a row in the data but with a numeric label`|`E`
`iterrows()` |`returning the index of the data and a series of each row`|`C` `E`  
`aggregate()` |`applying some aggregating function to some numerical columns`|`A`

$\rightarrow$ You may insert code snippets here if you like!

### 2. Pandas and NumPy 🔢 [BONUS 🎁](https://www.imdb.com/title/tt1068680/)

Pandas is built on top of the NumPy package, which means that many of the methods in NumPy are also available in Pandas. Data in pandas is often used to feed statistical analysis in SciPy, plotting functions from Matplotlib, and machine learning algorithms in Scikit-learn.

Speaking of NumPy, here are questions about it:

- What is the output of the following code? And why is it so?

<br/>
<br/>

<img align="right" src="https://media.giphy.com/media/OrKLdHysrpT89oZQ6A/giphy-downsized.gif" alt="Coder GIF" width="390" height="280">

``` python
a = np.array([1, 2, 3])
b = np.array([4, 5, 6])
c = np.vstack((a, b))

print(c[1][2])
```
``` python
[[1,2,3],
 [4,5,6]]
#As vstack puts the array on top of each other
```


- What is the output of the following code? And why is it so?

<br/>
<br/>

<img align="right" src="https://media.giphy.com/media/HwS1Xu5tQdUyGMYcBR/giphy.gif" alt="Coder GIF" width="390" height="280">

``` python
a = np.array([1, 2, 3])
b = np.array([4, 5, 6])
c = np.intersect1d(a, b)

print(c)
```
``` python
[]
#As the function finds the intersection between the two arrays which have nothing similar
```

  
- What is the output of the following code? And why is it so?

<br/>
<br/>

<img align="right" src="https://media.giphy.com/media/UNQ8B2nvmT5fhP9H5h/giphy.gif" alt="Coder GIF" width="390" height="280">

``` python
a = np.array([1, 2, 3])
b = np.array([4, 5, 6])
c = np.setdiff1d(a, b)

print(c)
```
``` python
[1,2,3]
# As the function finds the values in a not in b
```

- Which of the following is a function in NumPy used for carrying out Einstein summations?

    - [ ]  `np.tensordot()`
    - [ ]  `np.dot()`
    - [x]  `np.einsum()`
    - [ ]  `np.outer()`

- The `np.outer` function is primarily intended for:

    - [ ]  Computing the tensor dot product of two arrays.
    - [x]  Computing the outer product of two arrays.
    - [ ]  Computing the inner product of two arrays.
    - [ ]  Computing the cross product of two arrays.


### 3. Pandas and Matplotlib 📈
Pandas can be used to visualize data using a wrapper for `matplotlib.pyplot.plot()`. You can plot data directly from your DataFrame using certain functions.

- What functions can you use to plot data directly from your DataFrame? 🤔

 `plot()` `plot.line()` `plot.scatter()` `plot.bar()`
- What is the output of the following code? And why is it so?

``` python
df = pd.DataFrame(np.random.randn(10, 4), columns=['a', 'b', 'c', 'd'])
df.plot.scatter(x='a', y='b')
```
**>>>scatter plot each value of a and its corresponind value in b will be plotted**



- What do you know about `np.random.randn()`? And how does it depend on `np.random.seed()`?

`np.random.randn()` creates an array of specified size and fill it with real numbers

`np.random.seed()`  makes the random numbers predictable.look for this

``` pyhon
>>> numpy.random.seed(0)
>>> numpy.random.rand(4)
#the output
array([ 0.55,  0.72,  0.6 ,  0.54])
```
And if we run this again it will produce the same output.
but if we change the number in the seed function it will change the output
``` python
>>> numpy.random.rand(4)
#the output
array([ 0.42,  0.65,  0.44,  0.89])
```

## Git 🫴🏼
I know you are all familiar with Git, but let's see how much you know about it! 🤓

- What is the default text editor for the Bash shell with a Windows-based Git install?

    - [ ] Emacs
    - [x] Vim
    - [ ] Notepad++
    - [ ] Bash

- Before you install Git, which of the following prerequisite products must be present and configured on your local OS?

    - [ ] Python
    - [ ] Java Development Kit 1.8 or newer
    - [ ] Apache Maven
    - [x] Nothing


- After you install Git and prior to issuing the first commit, which two configuration properties does the tool expect to be configured?

    - [x] username and email address
    - [ ] username and password
    - [ ] email address and password
    - [ ] username and IP address

- Which of the following commands is used to create a new Git repository?

    - [x] git init
    - [ ] git clone
    - [ ] git commit
    - [ ] git push

- Which of the following commands is used to clone a remote Git repository?

    - [ ] git init
    - [x] git clone
    - [ ] git commit
    - [ ] git push

- Which of the following commands is used to stage a file for inclusion in the next commit?

    - [x] git add
    - [ ] git commit
    - [ ] git push
    - [ ] git pull

- Which of the following commands is used to commit staged changes to the local repository?

    - [ ] git add
    - [x] git commit
    - [ ] git push
    - [ ] git pull

- Which of the following commands is used to push committed changes to a remote repository?

    - [ ] git add
    - [ ] git commit
    - [x] git push
    - [ ] git pull

- Who is attributed with inventing Git?

    - [ ] Junio Hamano
    - [ ] James Gosling
    - [ ] Kohsuke Kawaguchi
    - [x] Linus Torvalds

- After you initialize a new Git repository and create a file named git-quiz.html, which of the following commands will not work if issued?

    - [ ] git add git-quiz.html
    - [ ] git status
    - [ ] git add .
    - [x] git commit -m "git quiz web file added"

- Which file can you configure to ensure that certain file types are never committed to the local Git repository?

    - [ ] ignore.git
    - [x] .gitignore
    - [ ] gitignore.txt
    - [ ] git.ignore

- Under which circumstance should you use a single dash within a bash command, as opposed to a double dash?

we may use single dash in short options and the double dash in long options


- Which vendor acquired GitHub for $7.5 billion in June 2018? `Microsoft`

You may want to check [this](https://www.youtube.com/watch?v=Q6G-J54vgKc&t=16813s)

## Problem Solving 🤔
[A. Panoramix's Prediction](https://codeforces.com/problemset/problem/80/A)

``` python
lis = [2,3,5,7,11,13,17,19,23,29,31,37,41,43,47,53,59]
num = (input()).split()
n = int(num[0])
m = int(num[1])
flag = False
for i in range(15) :
    if lis[i] == n and lis[i+1] ==m :
        flag = True
        break
if flag :
    print('YES')
else :
    print('NO')
```
[A. Again Twenty Five!](https://codeforces.com/problemset/problem/630/A)

``` python
n = intput()
print(25)
```
