---
layout: single
title: "About me"
author_profile: true
permalink: /
classes: wide
---
Hello! I'm Biying XU (徐毕颖), a first-year MPhil student in Computer Science and Engineering (CSE) at [the Hong Kong University of Science and Technology (HKUST)](https://hkust.edu.hk/). I am a member of the [HKUST VisLab](http://vis.cse.ust.hk/), under the supervision of [Prof. Huamin Qu](http://huamin.org/). I recently graduated with a Bachelor's degree in Software Engineering from [Zhejiang University](https://www.zju.edu.cn/) in June.
{: .text-justify}
My research is centered around **Data Visualization** and **Human-Computer Interaction (HCI)**. I am deeply fascinated by the potential of visualization to drive discovery in cross-disciplinary fields and am equally enthusiastic about exploring immersive interaction experiences through AR, VR, and MR. As an aspiring software developer, I find great fulfillment in building applications that address real-world problems, which is also a primary motivation behind my research.
{: .text-justify}
Beyond my academic pursuits, I am an avid painter, writer and reader. I cherish my diverse interests and am always eager to explore the boundaries and possibilities of my own life.
{: .text-justify}
I am always open to making new friends and collaborating on exciting research projects. Feel free to reach out to me via [email](mailto:bxuaw@connect.ust.hk)—I'd love to connect! (づ｡◕‿‿◕｡)づ
{: .text-justify}

## ✨ News

<ul class="news-list">
  {% assign sorted_news = site.data.news | sort: "date" | reverse %}
  {% for news in sorted_news %}
    <li class="news-item">
      <time class="news-date" datetime="{{ news.date }}">{{ news.date | date: "%Y.%m" }}</time>
      <div class="news-content">
        {{ news.message | markdownify | remove: '<p>' | remove: '</p>' }}
      </div>
    </li>
  {% endfor %}
</ul>
