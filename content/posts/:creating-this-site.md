---
title: "Creating this website with Hugo and Github"
date: 2020-12-29T23:49:25+05:30
slug: ""
description: ""
keywords: [hugo,github,static website,goat analytics]
draft: false
tags: [misc., tech]
math: false
comment: true
draft: false
toc: false
---

So I just finished publishing this website without errors and I thought I would document it here. To my pleasant surprise, It was pretty straightforward. 

I followed these steps:

1. I followed the first few steps directly from the [getting started guide of hugo](https://gohugo.io/getting-started/), where I installed it using `brew`, created an empty site and initialized it with `git`.

2. Now this second part is really really hard, which involves [choosing a theme](https://themes.gohugo.io/). Later I realized that it is very easy to switch between themes in hugo, so in retrospect, this shouldn't be that hard or time-consuming. I ended up choosing [hugo-coder](https://github.com/luizdepra/hugo-coder) which seems to be one of the more popular themes (i.e., more support and functionalities, yay!). [This report](https://github.com/TrentSPalmer/hugo_themes_report) from a random reddit post helped me make the decision.

3. I think the best way to add themes is using submodules (`git submodule add <github-url-for-the-theme> themes/<theme-name>`) even if the instructions say otherwise. I learned this the hard way but it is very easy to install multiple themes and switch between them using submodules. All the themes are stored in the /themes/ directory and you just need to change one line in the config.toml file. 

4. I created a github repository named [personal-blog](https://github.com/thehalfspace/personal-blog) and pushed this site to it.

5. I created another repository on github with the name thehalfspace.github.io (which would be <username>.github.io) to host the site. I found this technique pertty interesting where you host the rendered site in a different place (https://github.com/thehalfspace/thehalfspace.github.io) and the source material in a different place (https://github.com/thehalfspace/personal-blog). It makes so much sense to do this, but I didn't know of this before. In order to do this, we add the above hosting repository as a submodule to the `public/` directory. I pretty much followed [the official instructions](https://gohugo.io/hosting-and-deployment/hosting-on-github/) for hosting on github which didn't quite worked for me. For some reason, I had to change the step 6 to `git submodule add -b master https://github.com/thehalfspace/thehalfspace.github.io public`, but surprisingly, the branch name is `main`` when I change directory to public. The [deploy.sh](https://github.com/thehalfspace/personal-blog/blob/master/deploy.sh) is pretty cool which I run everytime I want to update stuff, and it automatically renders and pushes the changes to my hosting repository (https://github.com/thehalfspace/thehalfspace.github.io).

6. Now that my site is up and running, I want to add some extra stuff. I added [goat counter analytics](https://www.goatcounter.com/) which is a privacy friendly version of google analytics. Note that when using themes as submodules, you want to make changes to stuff in the `/themes/_theme-name_/folder` and not in the root of your site. So, in order to add goat analytics, copy the code into `/themes/hugo-coder/layouts/partial/analytics.html` or whatever your theme name is. 

This is all I have done so far, the next thing I want to do is add a view counter on the home page of the site. Goat analytics gives the script for that, I just need to figure out where to place it. I also need to add comments, disqus is the easiest choice, but I'll have a look at the alternatives before going forward with it. I'll update this section of the post once I have these changes ready. Finally, it would be nice to create and avatar to replace the stock avatar in my home page. I'll write about it in a subsequent post.

Peace,
( ͡° ͜ʖ ͡°)
