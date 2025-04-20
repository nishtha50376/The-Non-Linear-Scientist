---
layout: page
title: Science Topics 
permalink: /concepts/
---


This ASCII pattern represents rays converging to a focal point (center row), then diverging out — just like what you'd see in ray tracing or ZEMAX!


### 🐍 Python Code for ASCII Ray Simulation

```python
n = 3  # Beam size — increase for more rays

for i in range(2 * n + 1):
    if i < n:
        spaces = i
        gap = 2 * (n - i)
        print(' ' * spaces + '\\' + ' ' * gap + '|' + ' ' * gap + '/')
    elif i == n:
        print(' ' * n + '\\|/')
    else:
        spaces = 2 * n - i
        gap = 2 * (i - n)
        print(' ' * spaces + '/' + ' ' * gap + '|' + ' ' * gap + '\\')


# Next topic

Stroboscopic effect
