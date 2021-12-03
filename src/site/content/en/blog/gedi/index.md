---
layout: post
title: |
  GEDI case study: GEDI Digital improve mobile bounce rate by 8%
subhead: |
  By focusing development effort on performance improvement and applying the
  latest web technologies and techniques, GEDI Digital has created one of the
  fastest newspaper sites.
authors:
  - maurizioparadisi
date: 2021-12-10
hero: image/VbsHyyQopiec0718rMq2kTE1hke2/qg8rHQ5qlKK9t4Z6qTH2.jpeg
description: |
  By focusing development effort on performance improvement and applying the
  latest web technologies and techniques, GEDI Digital has created one of the
  fastest newspaper sites.
tags:
  - blog
  - case-study
  - web-vitals
---

## Introduction

Based in Rome, Italy, and formed in 1976, [GEDI](http://www.gedispa.it/) is a
media company that publishes 12 newspapers, several magazines, radio stations,
and 15 news sites. Their stable of publications includes
[La Stampa](https://www.lastampa.it/) and
[La Repubblica](https://www.repubblica.it/).

While GEDI is present in traditional publishing and broadcasting, its content
is increasingly being consumed on the web, and web is now contributing
significantly to their advertising revenue. Therefore, user retention and user
experience on the web are vital to the company’s overall prosperity.

## Challenge

According to Giuseppe Covato, Head of Innovation and New Technologies at GEDI
Digital, before 2017, they didn't have a strategic path for web performance.
Knowledge sharing between teams was minimal and inefficient. In particular, it
was hard to get marketing on board on technical topics such as Core Web Vitals.

With the introduction of Rep, a new premium content site, the Digital
team took the opportunity to experiment with emerging technologies such as
Polymer, AMP, and [progressive web apps](/progressive-web-apps/) (PWA). The
project also served as a playground to upscale the team around
performance-related objectives.

## Optimizations

To address performance, the team first applied critical rendering path
optimization, making sure there was no CSS or JavaScript that could slow down
the rendering time of editorial content.  This included deferring third-party
scripts and non-critical CSS, inlining critical CSS, and avoiding JavaScript
lazy loading on the first in-viewport images.

<figure>
{% Img src="image/VbsHyyQopiec0718rMq2kTE1hke2/h2MYvRTJMxFS4VrFRYTA.png",
   alt="26% improvement in time for LCP from Mar 1 through July 5",
   width="800", height="390"
%}
  <figcaption>
    Largest contentful paint (LCP) improvement trend
  </figcaption>
</figure>

The team then spent some time optimizing the site layout for stability by, for
example, reserving space for images based on their aspect ratio.

<figure>
{% 
   Img src="image/VbsHyyQopiec0718rMq2kTE1hke2/f5ZizQnDMyeFMDUJzmMj.png",
   alt="77% reduction in cumulative layout shift",
   width="800", height="390"
%}
  <figcaption>
    Cumulative Layout Shift improvement trend (first improvement by reserving space for Top Ads in Nov 2020, second improvement by reserving space for Mid page Ads by August 2021).
  </figcaption>
</figure>

## Results 

The new site became one of the fastest GEDI newspaper sites based on the key
metrics such as time to first byte and first content full paint. The team used
what they learned to scale this innovation to other high-traffic sites, such as
La Stampa and La Repubblica. 

<ul class="stats">
 <div class="stats__item">
   <p class="stats__figure">
     77
     <sub>%</sub>
   </p>
   <p>Reduction in CLS</p>
 </div>
 <div class="stats__item">
   <p class="stats__figure">
     26
     <sub>%</sub>
   </p>
   <p>Faster Largest Contentful Paint</p>
 </div>
 <div class="stats__item">
   <p class="stats__figure">
     8
     <sub>%</sub>
   </p>
   <p>Improved mobile bounce rate</p>
 </div>
</ul>

And, the benefits were measurable: on the La Repubblica mobile site, for
example, they measured a 77% reduction in [Cumulative Layout Shift](/cls/)
(CLS) and a 26%  improvement in time to [Largest Contentful Paint](/lcp/)
(LCP). Overall, the team found they reduced on La Repubblica's mobile bounce
rate by 8%.

The next step is to improve cumulative layout shift by minimizing the impact of
ads on site layout stability. Giuseppe considers this to be a big challenge
because they often deliver multi-site ad formats. Finding the right space to
serve is a challenge, a challenge that they are addressing by A/B testing
various solutions.  
