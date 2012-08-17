# Description

`njp` creates an empty skeleton file for a new post to be published via `jekyll`. I was tired of typing out the date and everything that has to be included in the file name whenever I created a new post.

Use it as follows:

~~~ sh
$ cd your_jekyll_dir/_posts
$ date
Fri Aug 17 20:23:26 CEST 2012
$ njp New tiny tool: njp
$ ls
2012-08-17-new-tiny-tool-njp.md
~~~

As you can see, `njp` will take all the command line options, strip them off non-alphanumerical characters, lowercase them, and concatenate them with hyphens.

There is a wee bit of content created, too:

~~~ markdown
---
layout: default
title: 'New tiny tool: njp'
---

# New tiny tool: njp
~~~

This is pulled from a heredoc within the script; if you want to make changes, change the script.

# Authors

* Thorsten Fischer (https://github.com/froschi)

# References

* Jekyll: https://github.com/mojombo/jekyll
