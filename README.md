# mmmlab_website

Welcome to our MMM lab website's GitHub page! Below is a brief tutorial on how to get started to edit our website on your own computer. 

## Step 1 - Getting started on Git

1. Open Rstudio on your computer. If you have yet downloaded Rstudio, please visit this https://rstudio.com/products/rstudio/download/#download. 

2. Go to "File" > "New Project". In the popped-up window, select "Version Control" > "Git" and put "https://github.com/winniewytse/mmmlab_website.git" under "Repository URL". 

3. There you go! You now have everything that is up on the remote Git repository on your local repository. 

4. Good habit 1: Every time before you start working on your local repository, remember to first **pull** the content from the remote repository by clicking on the blue downward arraow under "Git". 

5. Good habit 2: Every time after you made changes on your local repository, remember to **commit** the changes by clicking on "Commit" under "Git", checking all changed files, typing in a "Commit message", and "Commit". Then, click on the green upward arrow to **push** your changes to the remote repository. 

6. For more details, please check out https://happygitwithr.com/rstudio-git-github.html. 

## Step 2 - Getting started with `blogdown`

1. Install the `blogdown` package from either CRAN or GitHub. 

```r
## Install from CRAN
install.packages('blogdown') 
## Or, install from GitHub
if (!requireNamespace("devtools")) install.packages('devtools')
devtools::install_github('rstudio/blogdown')
```

2. Since blogdown is based on the static site generator Hugo (https://gohugo.io), you also need to install Hugo.

```r
blogdown::install_hugo()
```

3. You now have the access to all the functions and addins in `blogdown`. 

## Step 3 - Create/edit a post on our website

Under "Addins" (try to look for it on the top bar), there are multiple addins that come with `blogdown`, such as "Serve Site", "New Post", "Insert Image", etc. For details about the addins, please read https://bookdown.org/yihui/blogdown/rstudio-ide.html. 

1. To create a post, select "New Post" under "Addins". Put in details for 

    - Title: title of the post
    - Author: your name
    - Date: date when you create the post/publish the post, a choice of yours
    - Subdirectory: if you want your post to be showed under a subpage (e.g. research), put in the name of the subpage (i.e. research). 
    - Tags: add a tag on your post such that posts under the same tag are gathered together on our lab website for easier nevigations
    - Filename: it should be automatically generated after you put in details of above from the detail `post/YYYY-mm-dd-newfile.rmd`. 
    - Format: you can choose from "Markdown", "R Markdown (.Rmd)", or R Markdown (.Rmarkdown). Our default is R Markdown (.Rmd), which is the file format we are used to work under and has features that best fit our needs. 
        - For details of the differences among these file formats, please check out https://bookdown.org/yihui/blogdown/output-format.html. 
        
2. To edit a post, look for the file under "content" and its correponding files or folders. Start editing! Remember to always pull first before editing, and commit and push after editing. 

3. You are now good to go!

