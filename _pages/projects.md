---
layout: page
title: projects
permalink: /projects/
description: Projects across the broad areas of Sustainability and Data Tech.
nav: true
nav_order: 2
display_categories: [Imperial, ISO, BCI]
horizontal: false
---

<!-- pages/projects.md -->
<div class="projects">
{%- if site.enable_project_categories and page.display_categories %}
  <!-- Display categorized projects -->
  {%- for category in page.display_categories %}
  <h2 class="category">{{ category }}</h2>
  {%- assign categorized_projects = site.projects | where: "category", category -%}
  {%- assign sorted_projects = categorized_projects | sort: "importance" %}
  <!-- Generate cards for each project -->
  {% if page.horizontal -%}
  <div class="container">
    <div class="row row-cols-2">
    {%- for project in sorted_projects -%}
      {% include projects_horizontal.html %}
    {%- endfor %}
    </div>
  </div>
  {%- else -%}
  <div class="grid">
    {%- for project in sorted_projects -%}
      {% include projects.html %}
    {%- endfor %}
  </div>
  {%- endif -%}
  {% endfor %}

{%- else -%}
<!-- Display projects without categories -->
  {%- assign sorted_projects = site.projects | sort: "importance" -%}
  <!-- Generate cards for each project -->
  {% if page.horizontal -%}
  <div class="container">
    <div class="row row-cols-2">
    {%- for project in sorted_projects -%}
      {% include projects_horizontal.html %}
    {%- endfor %}
    </div>
  </div>
  {%- else -%}
  <div class="grid">
    {%- for project in sorted_projects -%}
      {% include projects.html %}
    {%- endfor %}
  </div>
  {%- endif -%}
{%- endif -%}
</div>



Project List

1. Mr. Cesar Maklary, Aeronautics MEng. Simulation of a Smart Grid, 2019. First Class Report. 
a. Industrial Cooperation with 100%Open and other Energy sector stakeholders.
2. Roman Kastusik, Aeronautics MEng. Automation and Intelligent Optimisation in High Performance Sailing Boats: Reinforcement Learning Approach, 2019. First Class Report.
a. Industrial Cooperation with T-DAB and other Sailing sector stakeholders.
3. Birk Andreas Ulstad, Aeronautics MEng. Automation and Intelligent Optimisation in High
Performance Sailing Boats: Supervised Learning Approach, 2019. First Class Report. a. Industrial Cooperation with T-DAB and other Sailing sector stakeholders.
4. Jason Tsai, MEng Computing. The Effect of Knowledge Graph Embeddings on Named Entity Disambiguation in Chatbots, 2019. First Class Report.
a. Industrial Cooperation with WisConT to support HSBC work.
5. Tim Green, BEng Computing. Industry Chat Bots: An investigation into current Named Entity Recognition models for automated chat bots and a proposed high-performance solution, 2019. First Class Report.
a. Industrial Cooperation with WisConT to support HSBC work.
6. Stanislas Hannebelle, MSc in Computing. Automation and Intelligent Optimisation in High
Performance Sailing Boats, 2019.
a. Industrial Cooperation with T-DAB and other Sailing sector stakeholders. Student
also attended the IoT Solutions World Congress in Barcelona.
7. Jiang Rong, MEng Computing. Multimodal Human Activity Recognition From Wearable Sensors and Video, First Class Report.
a. Industrial Cooperation with WisConT to support Chinese Business.
8. Alexander Gaskell, MSc Computing. On the Summarisation and Evaluation of Long
Documents, 2020. First-Class Report (Currently under review as conference paper). a. Industrial Cooperation with T-DAB to support other stakeholders.
9. Hamish Hall, MSc Computing. Graph Neural Networks for Classification of Ethereum Addresses and Analysis of Illicit Activity. First Class Report (Currently under review as conference paper).
a. Industrial Cooperation with WisConT.
10. Charles Metz, MSc Computing. Automation and Intelligent Control in High Performance
Sailing Boats, 2019. First Class Report.
a. Industrial Cooperation with T-DAB and other Sailing sector stakeholders. Student
also presented the work in 2020 Online IoT Solutions World Congress (normally will
be based in Barcelona).
11. Shaomiao Yin, MSc Computing. The Importance of IoT Data for Human Activity Recognition,
2019.
a. Industrial Cooperation with WisConT to support Chinese Business.



• “In particular, enormous gratitude is owed Pedro and Eric, whose time, knowledge and dedication to the project has proven crucial at countless points throughout. Roman and I would never have finished without you and your constructive criticism, guidance and patient understanding.” Birk A. Ulstad
• “I wish to express my special appreciation and thanks to my external and principal supervisor Dr. Pedro Baiz from WisConT. He has guided my work and encouraged my research throughout this project. By sharing his knowledge and putting me in contact with a range of energy industry and data science experts, he has been instrumental in the development of this paper as well as my future career. I would also like to thank the entire team from 100%Open, particularly Mr. David Simoes-Brown. They have set me in an ideal working environment to thrive during this project...” Cesar Maklary
• “I would like to thank Dr. Pedro Baiz for his continued support, feedback, and guidance throughout this project.” Tim Green
• “I would like to thank Dr. Pedro Baiz Villafranca for his continuous assistance through- out the duration of the project. He was always available to provide me with ideas and point me in a good direction for the project.” Jason Tsai
• ... “Firstly, huge gratitude is owed to Dr Pedro Baiz and Dr Eric Topham who, daily, gave a lot of their time, expertise and provided constructive criticisms and innovative ideas through- out this project. I feel extremely grateful for having the opportunity to be a part of the JTR AI project and wish the best of luck for future participants in this project. Also, I would like to particularly thank Jack Trigger for our regular communications and for sharing with me his navigation datasets.” ... Stanislas Hannebelle
• “I would like to thank the supervisor of this project, Dr. Pedro Baiz, who offers me a lot of help and guidance on this project.” Rong Jiang
• “I am grateful for the valuable help and insight I have received from a number of people affiliated with this project. I would first like to thank my supervisor, Dr. Pedro Baiz, for his guidance and insightful suggestions throughout. These have been invaluable for steering the direction of the project and helping me to always see the bigger picture. I would also like to thank The Data Analysis Bureau, T-DAB, and in particular Dr. Eric Topham and Hugo Barbaroux for your contributions to this project. You have each provided several important ideas which have helped shaped the project to what it currently is. Equally importantly, our frequent catch-ups helped maintain my sanity throughout the long Covid-19 dominated months without any access to the Imperial campus and regular human contact in general.” Alexander Gaskell.
• “I would like to thank my supervisors Dr. Pedro Baiz and Philip Nadler for their constant support and feedback throughout the project. I owe a lot of the structure of this project to their advice.” Hamish Hall
• “I would like to show my thanks to Dr. Pedro Baiz, who arranges meeting with me every week and give me suggestions on this project.” Shaomiao Yin
• “I would like to thank Roman Kastusik and Dr Eric Topham, who during almost five months took time for daily online meetings. Despite otherwise very full agendas, they were always available for enquiries and made me benefit very much from their experience, ideas and constructive criticism. I am particularly grateful that they did so during an era marked by a crown-shaped predator, on top of which they allowed me to gain insight into what was happening at their company T-DAB. I would also like to thank Dr Pedro Baiz, who contributed his input and knowledge to the project on a weekly basis; his feedback proved valuable in many ways.” Charles Metz
