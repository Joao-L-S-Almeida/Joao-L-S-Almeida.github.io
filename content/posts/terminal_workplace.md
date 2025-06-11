---
title: "Some tips for a better experience in the terminal"
featured_image: '/images/image_3.jpg'
date: 2025-06-10
draft: false
---

As most part of my daily work is passed in front of a terminal emulator I have continuously adapted my configuration (and adapted myself) to extract a smoother experience from it by avoiding distractions the best as possible. Here I list the tools I consider essential for my workflow and I encourage everyone to use too. There is no great novelty here, since all these tools are very popular and well-documented

# Fish

Since I start using [Fish](https://fishshell.com/) I always feel that something is missing when I use other shell. It manages the history in a way that makes the interaction with terminal very fluid and easy, since it automatically suggests possible completions for a command and lists others possibilities with the `CTRL+R` shortcut, almost like an auxiliary documentation for your daily workflow. In addition to this major characteristic, Fish also provides others simple and very helpful features, as underlining existent files, highlighting when a program is not installed and allowing the creation of new functions directly via CLI. All out of the box, without needing much configuration or extra plugins. 


# FZF

[FZF](https://junegunn.github.io/fzf/) is a command-line fuzzy finder which allows you to search for the location of a file by providing part of the file name. It works very well as a solitary tool, but it becomes even more useful in combination with others, as Vim and Zoxide. 

# Zoxide

The classical `cd` is excellent, but it has an inconvenience: it needs you remember the complete path for a directory. If the command is not memorized by Fish, for example, you will need at least to iteratively complete the path, which can be an annoying task when you need to to that multiple times per day. [Zoxide](https://crates.io/crates/zoxide) (in combination with FZF) comes to alleviate it by helping you to replace the long path with a shortcut or nickname. At the first time, you can use it in the same way as `cd`: 
```
z ~/dir/subdir/project
```
which will register the path and after it you can just type
```
z pro
```
and it will autocomplete or suggest a list of possibilities. What more could you want after that ?

Three is a good number. After start using these three tools, I believe you will feel your terminal is finally complete.
