# How to add a post

Each look is ONE file in `_posts/`, plus its three photos in `assets/images/<slug>/`.

1. Pick the slug: the look's name in lowercase with hyphens, e.g. `pink-plaid-pumpkin-patch-outfit`.
2. Photos: use each photo's full Higgsfield result URL (https://...png) as `src`. If the photo files can be saved into the repo instead, put them at `assets/images/<slug>/basic.jpg`, `styled.jpg` and `lifestyle.jpg` and use those paths. Both work.
3. Create `_posts/YYYY-MM-DD-<slug>.md` (date in America/Chicago) with the front matter below and nothing else.
4. Commit to the `main` branch and push. GitHub Pages rebuilds the site by itself in a minute or two.
5. The live post is at `https://bloomuponline.github.io/styleyourbestie/YYYY/MM/DD/<slug>/`.

The layout adds, by itself: the date, the "Shop the whole Idea List" buttons, an Amazon link for every piece in the form `https://www.amazon.com/dp/ASIN?tag=robinboateng-20`, the affiliate disclosure and the AI-generated images note. Do not write those into the file.

```yaml
---
layout: post
title: "The Pink Plaid Pumpkin Patch Outfit"
date: 2026-10-20 01:05:00 -0500
theme: "Fall pumpkin patch outfit"
intro: >-
  60 to 100 words in Robin's voice: first person, warm, funny, one real specific moment.
idea_list: "https://www.amazon.com/shop/bloomuponline.digitalproducts/list/XXXXXXXX"
photos:
  - src: /assets/images/pink-plaid-pumpkin-patch-outfit/basic.jpg
    alt: "Plain description of the Basic photo"
  - src: /assets/images/pink-plaid-pumpkin-patch-outfit/styled.jpg
    alt: "Plain description of the Styled photo"
  - src: /assets/images/pink-plaid-pumpkin-patch-outfit/lifestyle.jpg
    alt: "Plain description of the Lifestyle photo"
products:
  - name: "Short plain name"
    color: "Exact color or variant"
    asin: "B0XXXXXXXX"
---
```

Rules: photos are always in the order Basic, Styled, Lifestyle. Every piece of the look gets one `products` entry. Use quotes around any value that contains a colon.
