---
layout: post 
title: Legge til markdown 
parent: Referanse 
author: Simon
date: 23-01-06
nav_order: 1
---

```shell
_Ungdomskole/
├── content
└── Matematikk_8_trinn.md
_Universitet/
├── content
└── diskret_matematikk.md
_VGS
├── 1T.md
├── content
│   └── derivasjon.md
├── R1.md
└── R2.md
```

Midlertidig så er det tre forskjellige kataloger; og betegnes med en understrek "\_"
Disse katalogene vil du se til venstre, hvor navbaren ligger.

Her har vi en veldig lett forståelig struktur. 

La oss se på `_VGS` 

```shell
_VGS
├── 1T.md
├── content
│   └── derivasjon.md
├── R1.md
└── R2.md
```

Filene som har extention `.md` er markdown filer. 

Dersom du ønsker å legge til et nytt fag, så må `.md` være `_VGS/fag.md`

For `fag.md` så må det defineres en _front matter_

Front matter er noe som defineres først for en `.md`

#### Front matter

```markdown
---
layout: post
title: fag.md
author: Simon
date: 23-06-01
nav_order: 4
has_children: true
---
```

`layout: post` bruker en bestemt pre definert layout. 

{: .note}
> Dersom du skal legge til informasjon på denne nettsiden, behold `layout:post`  
> Dette gjør det sånn at du kan definere `author` og `date`
>
> En annen ting er at date formatet er år-dag-måned

`nav_order: 4` sier at den har indeks 4 i `_VGS`

Det er fint hvis du skriver dette, men dette trenges ikke. Dersom det er nødvendig, legg til.

`has_children: true` sier at `fag.md` er en foreldrer (parent)

I andre ord– så har den muligheten til å ha underkataloger.

Disse underkatalogene kalles for barn (children)

Alle underkataloger ligger i `/content/`

Front matter for en fil i `/content/` er nesten samme. Den eneste forskjellen her er at vi må definere en `parent`

Front matter for `/content/barn.md`, hvor den skal være en underkatalog for `_VGS/fag.md` (som vi lagde sist)

```shell
---
layout: post 
title: barn 
author: Simon
parent: fag 
nav_order: 1 
---
```
