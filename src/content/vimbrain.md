---
id: "vimbrain"
title: "VIM BRAIN"
group: "essay"
level: 2
val: 4
date: "2021-12-08"
tags: ["Vim", "Esoteric Languages", "Programming"]
links:
  - "programming"
---

[An obscure little project](https://github.com/salastro/vimBrain) that I finished recently was to create an esoteric programming language. My goal was to achieve the smallest possible set of vim-like instructions while being Turing-complete.

However, I am not the first one to try to do this. The first language to be Turing-complete with only 6 instructions was P′′ (P double prime) in 1964. Despite that, a variation from it created in 1993 got more popular. It was named Brainfuck (because it is incredibly frustrating) and added two more instructions for I/O.

Even with all of these variations floating around, there was no vim-inspired one, so I decided to make one. The rules themselves were simple to work out since it's a one-to-one mapping from Brainfuck; programming the interpreter was the part I actually enjoyed.

I decided that it should be written in as few lines as possible. That made me use Python instead of other programming languages I am familiar with because you can just compress the whole code into one line using semicolons in languages similar to C. Semicolons in Python, however, do not work in the same way: they create compound statements instead of terminating them.

After a couple of hours, the result was an interpreter function with only 17 lines of code. Everything from inline if-else statements to the new match-case statements was used to achieve this.

This was a fun one. It's refreshing to mess with niche concepts like this from time to time. Worth trying yourself if you want to see how you'd approach it, especially the loops, which are the tricky part.
