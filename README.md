### How to Make Changes to the Group Website

#### A. From your own forked repo

##### I. Getting Started

1. Fork the original [repo](https://github.com/az-digitalag/group-website)
2. If you do not already have RStudio installed, follow these [instructions](https://rstudio.com/products/rstudio/download/)
3. Open RStudio and navigate to your forked repo
4. If not already downloaded, install the blogdown and hugo packages using these [instructions](https://bookdown.org/yihui/blogdown/installation.html)
5. To preview the website locally, use the command `blogdown::serve_site()` in the console
6. You should now be able to preview the group website within RStudio, or copy and paste the url provided in the console into your browser. 

##### II. Keeping your forked repo up to date with new changes from the command line

1. From within your repo, check your currently configured remote repositories using `git remote -v`
2. If you only see your own repositories with your username, configure a new upstream repo with `git remote add upstream https://github.com/az-digitalag/group-website.git`
3. Check remote repositories again with `git remote -v`. You should now see the original az-digitalag repo in the list. 
4. Fetch all changes made to the original repo with `git fetch upstream`
5. If you are not already on your own `master` branch, switch to this branch with `git checkout master`
6. To merge changes from upstream/master to your own local master, use `git merge upstream/master`
7. To push the new changes to your github repo, use `git push origin master`

#### B. From a branch in az-digitalag/group-website repo
