---
title: "How i created my own Rust compiler"
date: 2023-08-19T15:55:04+02:00
draft: true
---

### Introduction

If you havent already read my blog post, which explains the basic concepts of a compiler, I would highly recommend you do [here](https://zyroz.dev/posts/compiler-explained/).

Before we get started, i want to quickly explain the goal i want to achieve. I am trying to create a rust compiler, but not to replace the extisting one, because I think its one of the greatest compilers ever, I only want to learn the concepts of a compiler in an real world example.

### Game Plan

- create a rust compiler which can check if there is a return type in the function, which is getting called.
- add support for expressions inside a function, which can also be inside the return statement, for example: return 1 + 2;
- add variable support and create an own typechecker which checks if all the potential of an intenger could even be used (if there is a function that uses a i64, but is only ever going to use numbers which are in the i32 range)

### **this blog post is work in progress, so thats why it isnt fully completed yet...**
