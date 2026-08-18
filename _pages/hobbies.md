---
layout: archive
title: "Hobbies"
permalink: /hobbies/
author_profile: true
---

A little collection of the hobbies I have acquired over the past few years...or decades

<style>
  /* Tiles are sized by aspect-ratio rather than fixed pixel heights, so every
     image keeps its proportions at any viewport width instead of being squashed. */
  .gallery {
    display: grid;
    gap: 12px;
    margin: 1.6em 0 2.4em;
  }
  .gallery.cols-3 {
    grid-template-columns: repeat(3, 1fr);
  }

  .gallery .tile {
    display: block;
    width: 100%;
    height: 100%;
    object-fit: cover;
    border-radius: 6px;
    box-shadow: 0 1px 5px rgba(0, 0, 0, 0.14);
    transition: transform 0.22s ease, box-shadow 0.22s ease;
  }
  .gallery .tile:hover {
    transform: translateY(-2px);
    box-shadow: 0 7px 20px rgba(0, 0, 0, 0.2);
  }

  /* Ratios chosen per photo so the crop stays close to the original framing. */
  .gallery .hero {
    aspect-ratio: 3 / 2;
    object-position: center 45%;
  }
  .gallery .banner {
    aspect-ratio: 16 / 9;
  }
  .gallery .portrait {
    aspect-ratio: 2 / 3;
  }
  .gallery .land {
    aspect-ratio: 4 / 3;
  }
  /* Near-square original: bias the crop upward to keep the lion's ears in frame. */
  .gallery .land.bias-up {
    object-position: center 38%;
  }

  /* Three narrow tiles stop being legible on a phone, so drop to one column. */
  @media (max-width: 640px) {
    .gallery.cols-3 {
      grid-template-columns: 1fr;
    }
    .gallery {
      gap: 10px;
    }
  }
</style>

Chinese Yo-Yo
======

I picked up the Diabolo or Chinese Yo-Yo over the last year and have been a part of
[Cornell Pro-Yos](https://www.instagram.com/cuproyos/), [Apex Diabolo](https://apexdiabolo.com/), and [Nova Diabolo](https://www.instagram.com/novadiaboloteam/). My most recent performances
were the [BU CSA Lunar New Year Gala](https://www.youtube.com/watch?v=hdVHol76xHo&t) and the [AANHPI Heritage Month Celebration](https://www.youtube.com/watch?v=8xJhbPJH74M).

<div class="gallery">
<img class="tile hero" src="/images/Apex.JPEG" alt="The Apex Diabolo team posing together at a performance" loading="lazy">
</div>

<div class="gallery cols-3">
<img class="tile portrait" src="/images/DoublesYoyo.jpeg" alt="Performing a doubles diabolo routine" loading="lazy">
<img class="tile portrait" src="/images/DiaboloInfinite.jpeg" alt="Tossing a diabolo high into the air" loading="lazy">
<img class="tile portrait" src="/images/nova.jpeg" alt="Performing with the Nova Diabolo team" loading="lazy">
</div>

Lion Dancing
======

For the last few years, I have studied lion dancing from [Cornell Lion Dance club](https://www.instagram.com/liondance_cornell/) and
[Mak-Fai Kung Fu and Lion Dance](https://www.makfailiondance.com/).

<div class="gallery">
<img class="tile banner" src="/images/liondance3.jpg" alt="A stage lined with lion dance teams mid-performance" loading="lazy">
</div>

<div class="gallery cols-3">
<img class="tile land bias-up" src="/images/liondance1.jpg" alt="Holding a white and blue lion head before a performance" loading="lazy">
<img class="tile land" src="/images/liondance2.jpg" alt="Lion dance performance in costume" loading="lazy">
<img class="tile land" src="/images/wmparade.jpeg" alt="The lion dance team in uniform at a Chinatown parade" loading="lazy">
</div>

To see me perform, check out [Mak Fai's 50th Anniversary Drum Routine](https://www.youtube.com/watch?v=WBAe_MTfots&t),
[ISU's Winter Gala Performance](https://www.youtube.com/watch?v=O8_vOy84bfA), or [CLD's showcase performance](https://www.youtube.com/watch?v=KlDutedmz_c).

[//]: # (Bridge)

[//]: # (======)

[//]: # ()
[//]: # (In my last year in undergrad, I picked up a little bit of bridge. I currently play Precision Club, and I'm)

[//]: # (on [bridge base online]&#40;https://www.bridgebase.com/&#41; under the name cs_ling.)

[//]: # ()

Linguistics
======
 
I like to dabble in linguistics, and some of my current topics of interest include syntactic topicalization, tonal languages, 
and the general field of pragmatics and semantics.

In my free time, I also enjoy learning and creating new languages. Languages that I am currently studying or have studied in the past include:

* Vietnamese
* French

And here are some languages I would like to study in the future:

* German
* Japanese
* Swedish
