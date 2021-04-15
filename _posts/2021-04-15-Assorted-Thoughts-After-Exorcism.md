---
layout: post
title: Assorted Thoughts After Ruby Exorcism and Helper Methods
---

Right now, we're consuming new Ruby topics through a firehose with a wide range of different work on various topics including learning Helper Methods and power of RESTful Routes as well as going through Ruby Exorcism excercises.  Below are a couple of interesting thoughts:


1.  The Power of .dig for Nested Ruby Hashes
    - During the Twelve Days Exorcism excercise, I decided to use a nested hash since each value in the loop (1..12) has two corresponding values ({placement: first, gift: "a partridge in a pear tree"}).  After nesting hashes, I needed an easy to use way to actually call down both layers of the hash to pull desired values when running through loops.  After some research I discovered .dig(arg1, arg2) which is explicitly built as a hash method that allows you to go down mulitple layers.  Hashes are extremely powerful in Ruby and I've had multiple areas where I've wanted to use nested hashes for certain situations previously, but couldn't because I didn't know the easy way to get to the inner hash.  With .dig I've found a new tool which will be very helpful in parsing information.   

2. Why write a loop to pull columns when you could just .transpose?
    - During the matrix exorcism assignment, the actual reading in process of the matrix (essentially read in and create nested array to hold rows) and returning a row was relatively simple, but when it came to taking the inverse (returning a column) I immediately defaulted to the brute force method of writing a loop.  After building something that I knew wasn't the most efficient I looked at solutions and discovered a solution that is not just 1 line succinct, it is one word succinct: .transpose.  Again, I was stunned at the simplicity and number of quick soultions Ruby has built-in.  

### Big Takeaway 

Don't reinvent the wheel - often there is a ruby method that can get you exactly what you want.  Exhaust your research first

