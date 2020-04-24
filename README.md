## How to Make Changes to the Group Website
_Note: All instructions with general git / github workflows can be moved / linked to OSF [pages](https://osf.io/tzmhp/wiki/home/)_

### A. From your own forked repo

#### I. Getting Started

1. Fork the original [repo](https://github.com/az-digitalag/group-website)
2. If you do not already have RStudio installed, follow these [instructions](https://rstudio.com/products/rstudio/download/)
3. Open RStudio and navigate to your forked repo
4. If not already downloaded, install the blogdown and hugo packages using these [instructions](https://bookdown.org/yihui/blogdown/installation.html)
5. To preview the website locally, use the command `blogdown::serve_site()` in the console
6. You should now be able to preview the group website within RStudio, or copy and paste the url provided in the console into your browser. 

#### II. Keeping your forked repo up to date with new changes from the command line

1. From within your repo, check your currently configured remote repositories using `git remote -v`
2. If you only see your own repositories with your username, configure a new upstream repo with `git remote add upstream https://github.com/az-digitalag/group-website.git`
3. Check remote repositories again with `git remote -v`. You should now see the original az-digitalag repo in the list. 
4. Fetch all changes made to the original repo with `git fetch upstream`
5. If you are not already on your own `master` branch, switch to this branch with `git checkout master`
6. To merge changes from upstream/master to your own local master, use `git merge upstream/master`
7. To push the new changes to your github repo, use `git push origin master`

#### III. How to add a team member to the People section

1. Within the repo in RStudio, open the `content` > `people` folders
2. Create a folder with the naming format of `new-person`
3. To include a photo or headshot in the bio, upload a `.png` image to that person's folder named `featured.png`
4. Copy `index.md` from another team member's folder and update with new information. Remember to change the team member tag to `current`, `affiliate`, or `past` as needed.
5. Commit and push your local changes to your forked repo and create a pull request in the original repo with these changes. 

#### IV. How to add a blog post

1. Within the repo in RStudio, open the `content` > `post` folders
2. As with the People section, copy an existing blog post and rename it using the `YYYY-MM-DD-name-of-post.md` format
3. Change the metadata at the top of the file as needed (i.e. `title`, `authors`, `date`, and `slug`)
4. Use Markdown [syntax](https://www.markdownguide.org/basic-syntax/) to write the post. 
5. Commit and push your local changes to your forked repo and create a pull request in the original repo with these changes. 

#### V. How to add images to a blog post
TBD (function that moves images automatically to the `static` folder?)

### B. From a branch in az-digitalag/group-website repo
