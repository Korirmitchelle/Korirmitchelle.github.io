---
layout: post
title: Difference between i++ and ++i
---


They both increment the number. ++i is equivalent to i = i + 1.

i++ and ++i are very similar but not exactly the same. Both increment the number, but ++i increments the number before the current expression is evaluted, whereas i++ increments the number after the expression is evaluated.

    int i = 6;
    int a = i++; // a = 6, i = 7
    int b = ++a; // b = 7, a = 7