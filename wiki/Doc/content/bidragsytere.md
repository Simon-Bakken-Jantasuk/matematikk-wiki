---
layout: post 
title: Legg deg selv som bidragsyter 
parent: Referanse 
author: Simon
date: 23-01-08
nav_order: 3
---
Dersom du har bidrat så har du muligheten til å legge deg selv på nettsiden som bidragsyter!

For å legge deg selv til så lag en yml fil,

#### Eksempel 

```shell
_data/
└── people
    └── simonbakkenjantasuk.yml
```

Dette er hva du har muligheten til å legge til,

```shell
- author: Simon
  email: simonbakkenjantasuk@pm.me
  social: 
    - matematikk.wiki
    - simonbakkenjantasuk.xyz

  donation: 46xCbLJLfvhFMDuKkLPiu7Th5DhbecMdyCPgzhL7KtVURQaskp3YfnYJ29vZdS6BtTXqfyneUwzPdNsEZiT9sFZANTNsg8T 
  gpg: simonbakkenjantasuk/public.key
```

Dersom dere ikke ønsker å legge til noe av dette, la oss si email. Så kan du velge å ikke legge til `email`

Dette gjelder de andre variablene i `.yml` filen.
