---
layout: page
title: About
permalink: /about/
author: Andrew
---

This is Andrew Harrison's internet homepage. It is chiefly about my personal interests as opposed to my work, but that's not to say that some work related matters won't creep in here from time to time.

## About the website
This is a static website that is written in [Markdown](https://www.markdownguide.org/) and built using the [Jekyll static site generator](https://jekyllrb.com/). The code for the website lives in a [GitHub repository](https://github.com/aharriso11/website), a local copy of which I keep on my [computer](https://www.apple.com/uk/mac-mini/). When I make changes to the website I push those changes from my computer to GitHub - I use [Visual Studio Code](https://code.visualstudio.com/) for making changes, creating posts and the integration with GitHub as it handles all these things out of the box.

The static web pages that are built from this code are actually hosted at and served from [Netlify](https://www.netlify.com/), which has its own [continuous deployment integration](https://www.netlify.com/blog/enhance-your-development-workflow-with-continuous-deployment/) with my GitHub repository to run the Jekyll `bundle exec jekyll build` command. I make do with the Netlify free tier which seems to work for the little traffic this site receives. The domain name and DNS are hosted by [Ionos](https://www.ionos.co.uk/).

The previous iteration of the site used [Wordpress](https://en-gb.wordpress.org/). This was served from a [Bitnami Wordpress template](https://bitnami.com/stacks/wordpress) hosted on [Amazon Lightsail](https://aws.amazon.com/lightsail/). This worked well enough but I did not really need the complication of Wordpress and its constant need to be kept up-to-date. I would have also had the additional future challenge of migrating the site to a new Wordpress template (thanks to the [deprecation of the Bitnami templates in Lightsail](https://community.broadcom.com/tanzu/blogs/beltran-rueda-borrego/2026/05/20/important-update-transitioning-bitnami-offerings-o)) which there isn't really a straightforward workflow for.