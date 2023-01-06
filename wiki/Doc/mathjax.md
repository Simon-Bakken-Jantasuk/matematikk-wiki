---
layout: post 
title: MathJax 
parent: Referanse 
author: Simon
date: 23-01-06
nav_order: 1
---
MathJax er en JavaScript library som viser matematikk på matematikk.wiki

MathJax er veldig lett å bruke. Det eneste du trenger er å skrive det i en markdown fil.

## Eksempeler 
$\int {sin(x)} dx = -cos(x) + C$

$lim_{x \to 0} \frac{sin(x)}{x} = 1$

Vi bruker enten `$$...$$` eller `$...$`

Dette er hvordan eksempelene over ser egentlig ut

Sett inn dette i den markdown fil, e.g barn.md som var lagd sist.

```
$\int {sin(x)} dx = -cos(x) + C$

$lim_{x \to 0} \frac{sin(x)}{x} = 1$
```

Sentrert ser slik ut

$$
\int {sin(x)} dx = -cos(x) + C
$$

$$
lim_{x \to 0} \frac{sin(x)}{x} = 1
$$

```
$$
\int {sin(x)} dx = -cos(x) + C
$$

$$
lim_{x \to 0} \frac{sin(x)}{x} = 1
$$
```
