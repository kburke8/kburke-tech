---
title: "Experimenting with Jekyll!"
date: 2021-01-01T15:34:30-04:00
categories:
  - blog
tags:
  - Jekyll
---

I recently stumbled upon Jekyll and Github Pages, and after more than a year of my original site being down, i decided to spin something up real fast and see what this stack is all about. I was shocked to find out how easy it was to pick a theme out and get started. For someone who is generally focused on the back-end side of things at work, it seemed like exactly what I needed.

I went through a number of different routes to try and get up and running, before eventually deciding upon a theme and the best route to take. Initially, I just went the most basic GitHub Pages route, which is to spin up a new repo, head over to the repo settings and enable GitHub Pages by selecting a branch for the site to mirror and choosing a theme. Setting up my custom domain was a piece of cake following the [directions][custom-domain-directions] and I pretty much instantly had a functioning site.

However, I quickly realized this was the most simple way to start a GitHub pages site with Jekyll, and that in the long run I may be better served choosing a more robust theme and standing up the repo myself. Well, it turns out, this is almost just as easy. After downloading the [requirements][jekyll-requirements] to run Jekyll locally, I simply had to: 
1. Install the Jekyll and Bundler Gems
 
     ~~~ shell
     gem install jekyll bundler
     ~~~
2. Create my site
 
     ~~~ shell
     jekyll new kburke-tech
     ~~~
3. Change to my new site's directory
 
     ~~~ shell
     cd myblog
     ~~~
4.  Build and run my site [step by step tutorial]
 
     ~~~ shell
     bundle exec jekyll serve
     ~~~
5.  Navigate to http://localhost:4000

After getting this going, I went through the basic [step by step tutorial] from the Jekyll documentation and felt like I had a pretty good idea of the overarching themes and syntax of the language. 

Around this time, I came across [Stackbit] and was intrigued at it's seemingly ease of use. However, after choosing my theme of choice, Jekyll as my static site generator, and Git as my Headless CMS, I found that the theme would not build on GitHub Pages and was given the incredibly informational "Page build failed" error with no additional details. The idea behind this error is that you will run the site locally and be given the true error, but when running locally I had no issues.

This was a reocurring issue across multiple stackbit approved themes, so I ultimately decided to move on from this.

So, What Did I Actually End Up Doing?
--------
At the end of the day, I found that the best way to get up and running on GitHub Pages with a full-fledged theme of my choice was to duplicate that themes starter template into a new repo and use that repo as opposed to the one I had done earlier. I ended up using the [Minimal Mistakes] jekyll theme as it seemed to be a popular one with a nice (optional) dark skin. 

[custom-domain-directions]: https://docs.github.com/en/free-pro-team@latest/github/working-with-github-pages/managing-a-custom-domain-for-your-github-pages-site#configuring-an-apex-domain
[jekyll-requirements]: https://jekyllrb.com/docs/installation/#requirements
[step by step tutorial]: https://jekyllrb.com/docs/step-by-step/01-setup/
[Stackbit]: www.stackbit.com
[Minimal Mistakes]: https://mademistakes.com/work/minimal-mistakes-jekyll-theme/