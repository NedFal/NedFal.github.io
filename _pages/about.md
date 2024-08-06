---
layout: about
title: about
permalink: /
subtitle: B.Sc. of Applied Mathematics & Computer Science at Sharif University of Technology

profile:
  align: right
  image: prof_pic.jpg
  image_circular: false # crops the image to make it circular
  more_info: >

news: false  # includes a list of news items
latest_posts: false  # includes a list of the newest posts
selected_papers: false # includes a list of papers marked as "selected={true}"
social: true  # includes social icons at the bottom of the page

preprints:
  title: "Emo3D: Translating Emotion Descriptions to 3D Facial Expressions, Benchmark Dataset and Evaluation Metrics"
  authors: "Mahshid Dehghani, Amirahmad Shafiee, Ali Shafiei, **Neda Fallah**, Farahmand Alizadeh, Mohammad Mehdi Gholinejad, Hamid Behroozi, Jafar Habibi, Ehsaneddin Asgari"
  date: "09 Apr 2024"
  summary: "The Emo3D paper introduces a novel dataset combining text, images, and 3D blendshapes to improve 3D facial emotion modeling. It proposes a new evaluation metric for better assessing visual-text alignment and semantic richness in 3D facial expressions."
  primary_subject: "Vision and Language"
  secondary_subjects: "Media Interpretation, Multimedia Foundation Models"
  pdf_url: "/assets/pdf/emo3d.pdf"
---

Hello!<br>

I hold a degree in Applied Mathematics and Computer Science from Sharif University of Technology.<br>
My primary interests lie in Natural Language Processing and Multimodal research, and I have actively participated in several projects within these fields.<br>

Download my <a href="https://github.com/NedFal/NedFal.github.io/blob/master/assets/pdf/nedcv.pdf" target="_blank"> CV</a>.<br><br>

### Preprint

**Title:** {{ page.preprints.title }}<br>
**Authors:** 
Authors: 
{% assign authors = page.preprints.authors | split: ',' %}
{% for author in authors %}
  {% if author contains 'Neda Fallah' %}
    {{ author }}{% unless forloop.last %}, {% endunless %}
  {% else %}
    {{ author }}{% unless forloop.last %}, {% endunless %}
  {% endif %}
{% endfor %}
**Submission Date:** {{ page.preprints.date }}<br>
**Summary:** {{ page.preprints.summary }}<br>
**Primary Subject Area:** {{ page.preprints.primary_subject }}<br>
**Secondary Subject Areas:** {{ page.preprints.secondary_subjects }}<br>
<a href="{{ page.preprints.pdf_url | relative_url }}" class="btn btn-primary" target="_blank">Preprint's PDF</a>

