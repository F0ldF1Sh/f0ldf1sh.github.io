---
layout: about
title: about
permalink: /
subtitle: >-
  An Undergraduate Student of <a href="https://en.uestc.edu.cn/">University of Electronic Science and Technology of China</a>

profile:
  align: right
  image: zheyu.jpg
  image_circular: false # crops the image to make it circular
  more_info: >
    <p style="font-size: 0.9rem; color: var(--global-text-color-light); margin-top: 0.5rem;">
      <a href="https://github.com/F0LDRA1N" target="_blank">GitHub</a> |
      <a href="/assets/pdf/zheyuwang_cv_zh.pdf" target="_blank">CV</a> |
      <a href="mailto:welda.z.wang@gmail.com"> Email</a>
    </p>

selected_papers: false # rendered manually below so honors can follow it
social: false # includes social icons at the bottom of the page

latest_posts:
  enabled: false
  scrollable: true # adds a vertical scroll bar if there are more than 3 new posts items
  limit: 5 # leave blank to include all the blog posts
---

I'm Zheyu Wang, a **final-year undergraduate student** majoring in Software Engineering at the **University of Electronic Science and Technology of China** (UESTC).

Currently, I'm a research intern in the Department of Psychological and Cognitive Sciences at Tsinghua University, working on foundation models for physiological signals.

My broader interests include **Generative Modeling**, **NeuroAI**, and **Computational Neuroscience**.

I will join the Department of Psychological and Cognitive Sciences at Tsinghua University as a Ph.D. student in Fall 2027. I'm always happy to discuss research ideas and potential collaborations!

<div style="clear: both"></div>

## experience

<div class="table-responsive">
  <table class="table table-sm table-borderless">
    {% assign experience = site.experience | sort: 'date' | reverse %}
    {% for item in experience %}
    <tr>
      <th scope="row" style="width: 25%">{{ item.period }}</th>
      <td>{{ item.content | remove: '<p>' | remove: '</p>' }}</td>
    </tr>
    {% endfor %}
  </table>
</div>

## news

{% include news.liquid %}

## selected publications

{% include selected_papers.liquid %}

## honors

<div class="table-responsive">
  <table class="table table-sm table-borderless">
    {% assign honors = site.honors | sort: 'date' | reverse %}
    {% for item in honors %}
    <tr>
      <th scope="row" style="width: 20%">{{ item.date | date: '%Y' }}</th>
      <td>{{ item.content | remove: '<p>' | remove: '</p>' }}</td>
    </tr>
    {% endfor %}
  </table>
</div>
