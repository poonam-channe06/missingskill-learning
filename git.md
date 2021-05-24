

<!-- Git Introduction -->
# git

* git is open source version control system.
* It tracks changes of your files
* It keeps your files well managed and maintained

<br/>
<!-- Github Branching -->

<p align="center"/><img src="Images\github_1.jpg" width="60%" />

<p align="center"/><img src="Images\github2_1.jpg" width="60%" />

<!-- What is repository -->
### __Repository__
<p align="center"/><img src="Images\repository _1.jpg" width="60%" />


<!-- Git and GitHub -->
### git vs  GitHub
<p align="center"/><img src="Images\gitvsgithub_1.jpg" width="60%" />

<br/><br/>

# git commands

<br/>
<p><strong>git init </strong>initializes and creates a new repository</p>

 <!-- git comands -->
```BASH
git init
```
<br/>

<p><strong>git config</strong> is used to config the local or global values</p>

```BASH
git config
```

<br/>

<p><strong>ex.</strong> Set the configuration files, such as username & email</p>

```BASH
git config --global user.email "poonam@gmail.com"
git config --global user.name "Poonam Channe"
```
<br/>

<p><strong>git add</strong> is used to add the file contents to the staging area</p>

```BASH
git add
```
<p></p>

```BASH
#  to add all files to staging area
git add . 

# adding particular file to staging
git index.html
git style.css
git app.js
```
<br/>


<p><strong>git commit</strong> is used save all the changes in the repository. 
   <strong>'-m'</strong> means message and next to it we write an appropriate message
</p>

<p>For example "adding project files","changing heading" etc.</p>


```BASH
git commit 
git commit -m "Any Message"
```
<br/>

<p><strong>git status</strong> will show all the files we have commited or the files that we have changed.</p>

```BASH
git status 
```
<br/>

<p><strong>git clone</strong> will copy the repository from existing URL </p>

```BASH
git clone (URL)
```
<br/>

<p><strong>git show</strong> will show a commit, log messages and a changes in the commit.</p>

```BASH
git show
```
<br/>

<p><strong>git log</strong> will display all of the previous commits in the repository. </p>

```BASH
git log
```
<br/>

<p><strong>git branch</strong> creates a new branch</p>

```BASH
git branch branch-name
```
<br/>

<p>If we want to switch to the other branch then we use the <strong>git checkout</strong>. For e.g git checkout dev, git checkout master/main.</p>


```BASH
git checkout branch-name
```

<p align="center"/><img src="Images\github_branching_1.jpg" width ="60%"/>

<p align="center"/><img src="Images\gothub_branching2_1.jpg" width ="60%"/>


<br/>
<br/>


<p><strong>git merge</strong>  merges all the individual branches into one single branch.</p>

```BASH
git merge
```
<br/>

<p><strong>git push</strong>  used to transfer or save  the local repository to the remote repository.</p>

```BASH
git push
```

<br/>

<p><strong>git  pull </strong>command allows us to pull the changes from the repository to local repository, if the changes has been made by someone else ex. when merging the pull request, we need to call <strong>git pull</strong> to reflect those changes on the local repository</p>

```BASH
git pull 
```

<br/>
<p align="center"/><img src="Images\github3_1 (1).jpg" width ="60%"/>



<!--  -->
