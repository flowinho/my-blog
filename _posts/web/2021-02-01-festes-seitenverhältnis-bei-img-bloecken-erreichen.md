---
title: "HTML IMG-Block: Fixes Seitenverhältnis ermöglichen"
layout: post
tags: .css
categories: ~/code
---

Wer trotz fix eingestellter `max-width` das Seitenverhältnis seiner Bild nicht ruinieren will, kann dies tun indem er die CSS-Proparty `object-fit` nutzt. 

Beispielhaft:

```css
img {
    max-height: 100px;
    max-width: 900px;
    object-fit: contain;
}
```