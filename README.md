# Udacious People Website 
## Table of Contents
* [Dependencies](#dependencies)
* [Installation](#installation)
* [Contributing](#contributing)
* [Running](#running)
* [Example](#example)


## Dependencies ##
In order build the website and develop it locally you need 
  * Git
  * Node.js
  * hexo-cli (via NPM)

## Installation ##
1. First fork the repository into your own profile. 
2. Clone the repo `git clone https://github.com/YOURUSERNAME/site.git`
3. `cd site`
4. `npm install`

Once you have your environment set up make sure you never deploy your site via hexo deploy because we will have a single person responsible for the [website](http://udaciouspeople.github.io).

For Documentation on Hexo.js go [here](https://hexo.io/docs/)

## Contributing ##
We welcome updates on the design and layout of the website along with new blog posts.

**All Blog Posts** must have a thumbnail and banner image as shown [here](#example)

## Running ##
In order to run a local instance of your work you must first generate the public repository and then serve it locally via these commands (run from the top directory):
```
hexo generate
hexo server
```
After you run `hexo generate`. The command  will get any debug code here if some configuration is wrong but it won't tell you if you have a messed up link for a photo or some other markdown mistake so make sure you check your work before submitting it.

## Example ##
To generate a new post or draft run `hexo new [layout] [url-title]` Where layout is either draft or post and the url-title is what you want the url path for the title of your blog post. Once you generate the proper markdown post/draft you will find it in `/source/_[layout]/[url-title]`
This is what a post page should look like:
```
title: [Title Name Pretty format]
date: [Date of creation]
thumbnail: [Image will be in assets/images/imageNAME.png but just put the image name here ]
banner: [Banner image if different from thumbnail, but must still be explicitly named]
category:
- [category]
tags:
- [tag1]
- [tag2]
---
[Your article goes here]
```
All images must be placed in a new folder with the title name 'title-other-stuff' to the folder sources/_post/title-other-stuff/ for you to have a thumbnail and cover image. [Here](https://github.com/LouisBarranqueiro/hexo-theme-tranquilpeak/issues/135) is a bug report where Louis Barranqueiro (the author of the theme) explains what to do about your images. 
You can also view a sample in source/_post/hello-world.md or view configuration details from the theme creater [here](https://github.com/LouisBarranqueiro/hexo-theme-tranquilpeak/blob/master/docs/user.md)
