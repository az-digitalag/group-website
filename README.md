## How to Make Changes to the Group Website
Note: General instructions for git / git workflow can be found on our group's OSF [page](https://osf.io/tzmhp/wiki/Using%20Git%20and%20GitHub/)


#### I. Getting started

1. Either clone the original [repo](https://github.com/az-digitalag/group-website) to your local computer and always work off of a non-master branch, or fork the original repo and clone the forked repo to your computer. You can additionally work off of a branch on the forked repo if you'll be working on multiple different tasks at a time. 
2. If you do not already have RStudio installed, follow these [instructions](https://rstudio.com/products/rstudio/download/)
3. Open RStudio and create a new project for your local cloned website repo
4. If not already downloaded, install the blogdown and hugo packages using these [instructions](https://bookdown.org/yihui/blogdown/installation.html)
5. To preview the website locally, use the command `blogdown::serve_site()` in the console
6. You should now be able to preview the group website within RStudio, or copy and paste the url provided in the console into your browser. 

#### II. How to add a team member to the People section

1. Within the repo in RStudio, open the `content` > `people` folders
2. Create a folder with the naming format of `new-person`
3. To include a photo or headshot in the bio, upload a `.png` image to that person's folder named `featured.png`
4. Copy `index.md` from another team member's folder and update with new information. Remember to change the team member tag to `current`, `affiliate`, or `past` as needed.
5. Commit and push your local changes to your forked repo and create a pull request in the original repo with these changes. 

#### III. How to add a blog post

1. Within the repo in RStudio, open the `content` > `post` folders
2. As with the People section, copy an existing blog post and rename it using the `YYYY-MM-DD-name-of-post.md` format
3. Change the metadata at the top of the file as needed (i.e. `title`, `authors`, `date`, and `slug`)
4. Use Markdown [syntax](https://www.markdownguide.org/basic-syntax/) to write the post
5. To add images to your blog post, use the `Add-ins` drop down menu within RStudio and select `Insert Image`
5. Commit and push your local changes to your forked repo and create a pull request in the original repo with these changes. 
