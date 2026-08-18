---
layout: archive
title: "CV"
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---

{% include base_path %}

<style>
  .cv-bar {
    display: flex;
    justify-content: flex-end;
    align-items: baseline;
    margin: -0.5em 0 1em;
  }
  .cv-bar a {
    font-size: 0.82em;
    letter-spacing: 0.03em;
    text-transform: uppercase;
    font-weight: 600;
    text-decoration: none;
    border-bottom: 1px solid transparent;
  }
  .cv-bar a:hover {
    border-bottom-color: currentColor;
  }
  .cv-bar .fas {
    margin-right: 0.4em;
  }

  /* Page-shaped so each PDF page fills the frame instead of letterboxing. */
  .cv-embed {
    display: block;
    width: 100%;
    aspect-ratio: 8.5 / 11;
    border: 1px solid #dcdcdc;
    border-radius: 3px;
    box-shadow: 0 2px 14px rgba(0, 0, 0, 0.08);
    background: #f4f4f4;
  }

  .cv-fallback {
    display: none;
  }

  /* Mobile browsers largely refuse to render inline PDFs — send them to the file. */
  @media (max-width: 768px) {
    .cv-embed {
      display: none;
    }
    .cv-fallback {
      display: block;
      padding: 1.4em 1.5em;
      border: 1px solid #dcdcdc;
      border-radius: 3px;
      background: #f8f8f8;
      text-align: center;
    }
    .cv-fallback .btn {
      margin-top: 0.6em;
    }
  }
</style>

<div class="cv-bar">
  <a href="{{ base_path }}/files/CV_Tia_Vu.pdf"><i class="fas fa-download" aria-hidden="true"></i>Download PDF</a>
</div>

<object class="cv-embed" data="{{ base_path }}/files/CV_Tia_Vu.pdf" type="application/pdf">
  <div style="padding:1.4em 1.5em;text-align:center;">
    Your browser can't display PDFs inline.
    <a href="{{ base_path }}/files/CV_Tia_Vu.pdf">Download the CV</a> instead.
  </div>
</object>

<div class="cv-fallback">
  Inline preview isn't available on small screens.
  <a class="btn btn--info" href="{{ base_path }}/files/CV_Tia_Vu.pdf">Download CV (PDF)</a>
</div>
