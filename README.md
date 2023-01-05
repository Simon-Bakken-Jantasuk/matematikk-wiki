# Matematikk.wiki 

Hvis du ønsker å legge til innhold så lag en "_pull request_"

Les mer om dette på [How to create a pull request?](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/creating-a-pull-request)


# Hvordan legge til innhold?

```
.
├── assets
│   └── js
│       └── yearChanger.js
├── _config.yml
├── Gemfile
├── Gemfile.lock
├── _includes
│   ├── footer_costum.html
│   ├── nav_footer_custom.html
│   └── toc_heading_custom.html
├── index.md
├── LICENSE
├── README.md
├── ressurs
│   └── index.md
└── wiki
    ├── Ungdomskole
    │   └── index.md
    ├── Universitet
    │   └── index.md
    └── VGS
        ├── 1T.md
        ├── index.md
        ├── R1.md
        └── R2.md
```

Midlertidig, så er det 3 forskjellige kataloger.

1. Ungdomskole
2. VGS
3. Universitet

Ved alle av disse katalogene så er det en `index.md` og alle av dem har `has_children: true` i sin front matter. 
Dette er for å betegne at katalogene er foreldrer (parent)

Ønsker du å legge til et nytt fag? Så lager du en markdown fil med fagets navn.

La oss se på `R1.md`

```
---
layout: default
title: R1 
parent: VGS 
nav_order: 2
has_children: true
---
Vurderingskriterier
```

Her har vi en `layout: default`, som er den du skal bruke. Tittel er tittelen til faget. Parent vil betegne foreldrer, 
som er VGS. Vi vet dermed at `R1.md` er ett barn. `Nav_order` sier seg selv, dette er indeksen. `Has_children` vil si at 
`R1.md` er en foreldrer (parent)

I tillegg så ønsker jeg at det er vurderingskriterier for fagene.

Likevel, sånn her kan du fortsette. Ønsker du å ha en under katalog, eller barn for foreldrer R1? 

Så kan du foreksempel lage en ny markdown fil, med ny front matter.

Den kan se sånn her ut

```
---
layout: default
title: Derivasjon
parent: R1 
nav_order: 1
---
Skriv her...
```

