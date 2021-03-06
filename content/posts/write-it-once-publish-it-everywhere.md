---
date: 2020-04-18T00:27:41.000+00:00
title: Write it Once, Publish it Everywhere
author: Kerrbear
tags:
- web publishing
- api
- automation
- deployment
title_main: Deterministic Publishing Robot Design and Development
title_sub: or How to Post on Forestry and have Github, Zeit, IFTTT, and Medium Do Their
  Thangs
title_lead: Could've built a better mousetrap, but hey…
categories: []
draft: true

---
Writing has become effortless. Now I would love to simplify my publishing process. With any luck, I might be able to reach readers eventually.

Ideally I can:

1. Write a post through the WYSIWIG/Markdown editor on Forestry.io.
2. Have Forestry auto-publish the post and sync it to the Github repo.
3. Have the Hugo deployment hosted on Zeit Now listen for pushes to the repo and update the site with the new post.
4. Have IFTTT watch the RSS feed for the site and send a POST to through the Medium API to add the post to the Atmanautica publication on Medium.

So far I've got the first three working, and the fourth step is wired up, but so far unsuccessful.