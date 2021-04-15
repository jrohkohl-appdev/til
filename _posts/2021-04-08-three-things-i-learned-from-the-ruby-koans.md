---
layout: post
title: Three things I learned from The Ruby Koans
---

Here are (at least) three things I learned from [The Ruby Koans](http://rubykoans.com/):


1. Symbols, Messages, and a few other topics were completely unheard of topics to me prior to the exercise, it was interesting to get exposure.
2. There are so many better ways to search within objects for specific text or values.  Methods like .find_all and regular expressions were extremely useful in parsing information.
3. The usefulness of Regular Expressions - Ruby has extremely granular tools to parse text files and they can be incredibly powerful... but they also can be tricky.  For example, code such as matrix.append(selected_row.split(/[\D]+/).map {|num| num.to_i}) confusingly will not remove leading spaces (i.e. " 6, 7, 8, 9" which will produce "" as one of the splits)
