---
layout: post
title: "Jekyll blog 30 minute mein kaise banao"
date: 2024-03-20
tags: [jekyll, github, tutorial]
excerpt: "GitHub Pages pe free mein blog kaise host karein — step by step guide Urdu mein."
---

Bhai, sach batao — blog banana utna mushkil nahi jitna lagta.
## Kya chahiye?

- GitHub account (free)
- Thoda patience

## Steps

1. Is repo ko fork karo
2. Repo ka naam rakho: `TUMHARA-USERNAME.github.io`
3. Settings > Pages mein jao
4. Branch `main` select karo
5. Save karo — bas!

Kuch minutes mein aapka blog live hoga.

## `_config.yml` update karo

Ye zaroor karo:

```yaml
title: "Tumhara Blog Naam"
author: "Tumhara Naam"
url: "https://TUMHARA-USERNAME.github.io"
```

## Naya post kaise likho?

`_posts/` folder mein file banao is format mein:

```
YYYY-MM-DD-post-title.md
```

Upar yeh likho:

```yaml
---
layout: post
title: "Mera Naya Post"
date: 2024-03-20
tags: [tag1, tag2]
---
```

Phir apna content likho. Itna hi!
