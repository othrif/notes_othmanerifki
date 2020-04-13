---
# Documentation: https://sourcethemes.com/academic/docs/managing-content/

title: "Looping Over Two Lists"
description: "Looping over two lists using Python."
author: "Othmane Rifki"
subtitle: ""
summary: ""
authors: []
tags: []
categories: []
date: 2020-04-10T20:58:27+02:00
lastmod: 2020-04-10T20:58:27+02:00
featured: false
draft: false

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder.
# Focal points: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight.
image:
  caption: ""
  focal_point: ""
  preview_only: false

# Projects (optional).
#   Associate this post with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `projects = ["internal-project"]` references `content/project/deep-learning/index.md`.
#   Otherwise, set `projects = []`.
projects: []
---
```python
# Create a list of length 3:
armies = ['Red Army', 'Blue Army', 'Green Army']

# Create a list of length 4:
units = ['Red Infantry', 'Blue Armor','Green Artillery','Orange Aircraft']
```


```python
# For each element in the first list,
for army, unit in zip(armies, units):
    # Display the corresponding index element of the second list:
    print(army, 'has the following options:', unit)
```

    Red Army has the following options: Red Infantry
    Blue Army has the following options: Blue Armor
    Green Army has the following options: Green Artillery

Notice that the fourth item of the second list, `orange aircraft`, did not display.

```python
# Import modules
import numpy as np
```


```python
# Create a list
battle_deaths = [3246, 326, 2754, 2547, 2457, 3456]
battle_deaths
```




    [3246, 326, 2754, 2547, 2457, 3456]




```python
# Create an array from numpy
deaths = np.array(battle_deaths)
deaths
```




    array([3246,  326, 2754, 2547, 2457, 3456])




```python
# Create an array of zeros
defectors = np.zeros(6)
defectors
```




    array([ 0.,  0.,  0.,  0.,  0.,  0.])




```python
# Create a range from 0 to 100
zero_to_99 = np.arange(0, 100)
zero_to_99
```




    array([ 0,  1,  2,  3,  4,  5,  6,  7,  8,  9, 10, 11, 12, 13, 14, 15, 16,
           17, 18, 19, 20, 21, 22, 23, 24, 25, 26, 27, 28, 29, 30, 31, 32, 33,
           34, 35, 36, 37, 38, 39, 40, 41, 42, 43, 44, 45, 46, 47, 48, 49, 50,
           51, 52, 53, 54, 55, 56, 57, 58, 59, 60, 61, 62, 63, 64, 65, 66, 67,
           68, 69, 70, 71, 72, 73, 74, 75, 76, 77, 78, 79, 80, 81, 82, 83, 84,
           85, 86, 87, 88, 89, 90, 91, 92, 93, 94, 95, 96, 97, 98, 99])




```python
# Create 100 ticks between 0 and 1
zero_to_1 = np.linspace(0, 1, 100)
zero_to_1
```




    array([ 0.        ,  0.01010101,  0.02020202,  0.03030303,  0.04040404,
            0.05050505,  0.06060606,  0.07070707,  0.08080808,  0.09090909,
            0.1010101 ,  0.11111111,  0.12121212,  0.13131313,  0.14141414,
            0.15151515,  0.16161616,  0.17171717,  0.18181818,  0.19191919,
            0.2020202 ,  0.21212121,  0.22222222,  0.23232323,  0.24242424,
            0.25252525,  0.26262626,  0.27272727,  0.28282828,  0.29292929,
            0.3030303 ,  0.31313131,  0.32323232,  0.33333333,  0.34343434,
            0.35353535,  0.36363636,  0.37373737,  0.38383838,  0.39393939,
            0.4040404 ,  0.41414141,  0.42424242,  0.43434343,  0.44444444,
            0.45454545,  0.46464646,  0.47474747,  0.48484848,  0.49494949,
            0.50505051,  0.51515152,  0.52525253,  0.53535354,  0.54545455,
            0.55555556,  0.56565657,  0.57575758,  0.58585859,  0.5959596 ,
            0.60606061,  0.61616162,  0.62626263,  0.63636364,  0.64646465,
            0.65656566,  0.66666667,  0.67676768,  0.68686869,  0.6969697 ,
            0.70707071,  0.71717172,  0.72727273,  0.73737374,  0.74747475,
            0.75757576,  0.76767677,  0.77777778,  0.78787879,  0.7979798 ,
            0.80808081,  0.81818182,  0.82828283,  0.83838384,  0.84848485,
            0.85858586,  0.86868687,  0.87878788,  0.88888889,  0.8989899 ,
            0.90909091,  0.91919192,  0.92929293,  0.93939394,  0.94949495,
            0.95959596,  0.96969697,  0.97979798,  0.98989899,  1.        ])


```python
# Create a list of length 3:
armies = ['Red Army', 'Blue Army', 'Green Army']

# Create a list of length 4:
units = ['Red Infantry', 'Blue Armor','Green Artillery','Orange Aircraft']
```


```python
# For each element in the first list,
for army, unit in zip(armies, units):
    # Display the corresponding index element of the second list:
    print(army, 'has the following options:', unit)
```

    Red Army has the following options: Red Infantry
    Blue Army has the following options: Blue Armor
    Green Army has the following options: Green Artillery


Notice that the fourth item of the second list, `orange aircraft`, did not display.