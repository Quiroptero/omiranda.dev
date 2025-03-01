---
title: "A file structure to quickly develop a Hugo theme"
subtitle: ""
summary: ""  # This one is displayed in the list of posts

date: 2024-11-29T11:14:26-06:00
lastmod: 2024-11-29T11:14:26-06:00

slug: ""

tags: []

draft: true
---

This one intends to demonstrate the benefits of having a git worktree 
for your blog, with a branch pointing to main and another branch pointing to draft.
Inside the draft one, in the themes folder, a symlink pointing to other git repo for your Hugo theme.
<!--more-->

make this one with a demonstration:

assume git repos in github, but make clear that same file structure works without github (reader homework to set it up)

mkdir website
cd website
git clone website main
cd source
git worktree add ../draft
git clone theme
cd draft
symlink to theme
