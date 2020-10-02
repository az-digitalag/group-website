## How to Make Changes to the Group Website
Note: General instructions for git / git workflow can be found on our group's OSF [page](https://osf.io/tzmhp/wiki/Using%20Git%20and%20GitHub/)

Any changes that are merged into the master branch of this repo are automatically published to the website. 

#### I. Getting started

1. Either clone the original [repo](https://github.com/az-digitalag/group-website) to your local computer and always work off of a non-master branch, or fork the original repo and clone the forked repo to your computer. You can additionally work off of a branch on the forked repo if you'll be working on multiple different tasks at a time. 
2. If you do not already have RStudio installed, follow these [instructions](https://rstudio.com/products/rstudio/download/)
3. Open RStudio and create a new project for your local cloned website repo
4. If not already downloaded, install the blogdown R package and Hugo using these [instructions](https://bookdown.org/yihui/blogdown/installation.html)
5. To preview the website locally, use the command `blogdown::serve_site()` in the console
6. You should now be able to preview the group website within RStudio, or copy and paste the url provided in the console into your browser. 

#### II. How to add a team member to the People section

1. Within the repo in RStudio, open the `content` > `authors` folders
2. Create a folder with the naming format of `firstname-lastname`
3. To include a photo or headshot in the bio, upload a `.png` image to that person's folder named `avatar.png`
4. Copy `_index.md` from another team member's folder and update with new information. Remember to: update `Display name`, `Role/position`, and `Social/Academic Networking`; set `user_groups` to "Current Members", "Affiliates", or "Alumni"; and add a paragraph or two about the person's interests, role in the group, and past experiences at the end after the yml. 
5. Run `blogdown::serve_site()` in the RStudio console and check social media links are correct on new person page

#### III. How to add a blog post

**Automatically:** 
-  `Addins` > `new post` or `blogdown::new_post()`
  - this provides handy arguments including title, author, tags, date, and file that will be used to populate the new post. 
  
**Manually:**
1. Within the repo in RStudio, open the `content` > `post` folders
2. As with the People section, copy an existing blog post and rename it using the `YYYY-MM-DD-name-of-post.md` format
3. Change the metadata at the top of the file as needed (i.e. `title`, `authors`, `date`, and `slug`)
4. Use Markdown [syntax](https://www.markdownguide.org/basic-syntax/) to write the post
5. To add images to your blog post, use the `Add-ins` drop down menu within RStudio and select `Insert Image`

#### IV. How to add a publication

The content for each publication goes in a folder `content/publication/author-YYYY`.

This folder can be generated automatically from a bibtex file. Most reference management software and search portals (e.g. Mendeley, Zotero, Google Scholar) provide an option to export a citation as bibtex. There is a tool to automatically generate the folder, index.md, and cite.bib files for each publication using the shell command `academic import --bibtex <path_to_your/publication.bib>` following [the Academic Hugo documentation](https://sourcethemes.com/academic/docs/managing-content/#create-a-publication))

A minimal set of yaml header fields are described in the [documentation](https://sourcethemes.com/academic/docs/managing-content/#manually). We have changed the default publication type 8 to be data publications by editing `data/publication_types.toml` and `i18n/en.yaml` as described in the documentation. 

Recommended fields to include in the index.md:  
* `publication_types: ["8"]` 
  1 = conference proceedings
  2 = journal article
  8 = data publication (this is different than default for 8)
* `doi`
* `url` to website for related project; do not include `https://`.

Also:
* To add a featured image: place an image file named `featured.*` in the publication (`publications/author-YYYY`) directory. 
