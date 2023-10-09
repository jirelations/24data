---
layout: reveal
title: "Slide Test"
author: "Nathan Gibson"
categories: sample
tags: [1,slides]
image: arctic-1.jpg
parallaxBackgroundImage: 'assets/img/arctic-1.jpg'
---

## Flex CSS with Stretch

{% include img-row.html images="assets/img/cuba-2.jpg,assets/img/cuba-1.jpg,assets/img/cuba-2.jpg" %}

This is how you can include a row of images that automatically fills the width of the slide. By default, the `include` uses the `r-stretch` class from revealJS to set the row height. If you have a lot of text like this, the row will adjust. You can also include the "class" parameter with a row and number (out of 12) to set the row height (e.g., `class="row-2"`).