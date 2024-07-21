---
layout: default
title: Projects
---

<meta content="{{ site.title }}" property="og:site_name">
{% if page.title %}
  <meta content="{{ page.title }}" property="og:title">
{% else %}
  <meta content="{{ site.title }}" property="og:title">
{% endif %}
{% if page.title %}
  <meta content="article" property="og:type">
{% else %}
  <meta content="website" property="og:type">
{% endif %}
{% if page.description %}
  <meta content="{{ page.description }}" property="og:description">
{% else %}
  <meta content="{{ site.description }}" property="og:description">
{% endif %}
{% if page.url %}
  <meta content="{{ site.url }}{{ page.url }}" property="og:url">
{% endif %}
{% if page.date %}
  <meta content="{{ page.date | date_to_xmlschema }}" property="article:published_time">
  <meta content="{{ site.url }}/about/" property="article:author">
{% endif %}
{% if page.image %}
  <meta content="/img/srcset/{{ page.image }}" property="og:image">
{% else %}
  <meta content="/img/logo-high-resolution.png" property="og:image">
{% endif %}
{% if page.categories %}
  {% for category in page.categories limit:1 %}
  <meta content="{{ category }}" property="article:section">
  {% endfor %}
{% endif %}
{% if page.tags %}
  {% for tag in page.tags %}
  <meta content="{{ tag }}" property="article:tag">
  {% endfor %}
{% endif %}

* * *
### Projects[`ICARE`]
* * *
![FIDC]({{ '../../assets/images/Asset 22.png' | relative_url }})
# INTRODUCTION
Bismillah🤲<br/>
Hello good day, Welcome to my blog. I'm <st style="color: rgb(0, 210, 45);">spectra</st> thanks for visiting my blog,I really appreciate. I'm a software engineer, I love to code and I'm a problem solver. I'm also a <b style="color: rgb(255, 166, 0);">python3 Freak 🤠</b>. I developed the Backend of this project with two of my favorite tech Buddies <a href="https://github.com/chocolaid">Emmanuel(Mobile App Development)</a>and <a href="https://www.linkedin.com/in/habeeb-oke-8569a7248">Habeeb Oke(Frontend Developer)</a>.<br/>
# What's is Icare
Icare(i.e Interactive Care) is an Artificial Intellegence Mobile application that leverages Ai capabilities to attend to critical Emergency Situations 
# Features
Icare has tons of features built with it:
1. Emergency Response Ui - This enables users to quickly interact with the Ai As fast as possible because of our Simple Ui
2. Skin Cancer Classification Model - This enables our users to use our skin cancer classification Model to be able to predict skin cancers From skin lesions
3. Interactive Ai(Jarvis) - Users can interact with our Pre-Prompted Medical Ai for quick Medical tips 
4. High Accuracy: Utilizes state-of-the-art deep learning algorithms.<br/>
5. User-Friendly: Easy integration with existing healthcare systems.<br/>
6. Scalable: Can be deployed on multiple devices and platforms.<br/>

# Tech Stack - Technologies
**Front-End Technologies**<br/>
    - Purpose: To create the user interface and user experience of an application.<br/>
    - Design: React Native<br/>
**Back-End Technologies**<br/>
    - Purpose: To handle server-side logic, database interactions, and application functionality.<br/>
    - Programming language: Python <br/>
    - Framework: Flask<br/>
**Database Technologies**<br/>
    - Purpose: To store, retrieve, and manage application data.<br/>
    - Database: SQLite, Firebase<br/>

# PROJECT VIEW
<img src="{{ '../../assets/images/icare_home.jpg' | relative_url }}" alt="Icare Home" width="20%" height="auto">
<img src="{{ '../../assets/images/Icare_Inbox.jpg' | relative_url }}" alt="Icare Inbox" width="20%" height="auto">
<img src="{{ '../../assets/images/Icare_news.jpg' | relative_url }}" alt="Icare News" width="20%" height="auto">
<img src="{{ '../../assets/images/Icare_directions.jpg' | relative_url }}" alt="Icare Directions" width="20%" height="auto">

### **[Home]({{ '../../' | relative_url }})**