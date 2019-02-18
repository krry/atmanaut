---
title: README
date: 2019-02-02 02:22:22 -0600
---

# Atmanaut

Spelunk the essential.

### This is:
A hugo-powered static site using the chakra theme, ready to link up with a
Forestry.io CMS, and auto-deployable on now.sh.

## TODO
- [ ] flesh out tagging system for asidebar and posts
- [ ] scour hugo docs and try out features
- [ ] refresh color palette: chakras, soulstones
- [ ] consider annotation lane for links and sidenotes (a la footnotes)
- [ ] learn how to direct link to other posts
- [x] style summaries: timestamps, titles, etc.
- [x] add routes to `now.json` to enable Github master push deploy
  - move `now.json` back to root
  - change npm scripts to work with new build config
- [x] add logo

## Tagging, Categories, and Taxonomies

Hugo provides two [default taxonomies](https://gohugo.io/content-management/taxonomies/#default-taxonomies): tags and categories. Additional taxonomies can be added in the `config.yaml` like so:
``` yaml
taxonomies:
  example: examples
  thing: things
```
Then you can use it in `YAML` front matter like so:
``` md
---
title: An article por ejemplo
things: bunnicula, flying saucers
tags: punishment, acrobatics
---
```
Each taxonomies type gets its own page (e.g. `/categories`, `/tags`) and each term in the taxonomy gets a page listing all its members (e.g., `/tags/horsenames`).

## Linking to posts

Hugo provides `relURL` and `absURL` for your linking needs. These power `.RelPermalink` and `.Permalink` respectively.

Use .RelPermalink when you might alter the locations of the `publicDir` or `contentDir`, or restructure the dynamically generated `[permalinks]` in the site `config.toml`.

Use .Permalink when the file won't move, or for external purposes, such as sharing and for post title links.

