---
title: "Bristol Glaciology Centre"
# excerpt: "This puts a subtitle on the header image, if we want one"
layout: splash
permalink: /
author_profile: false
header:
  overlay_color: "#000"
  overlay_filter: "0.1"
  overlay_image: /assets/images/headers/header_fracture.jpg
feature_row:
  - image_path: https://placehold.co/400x300?text=Research
    title: "Research"
    excerpt: "Explore our multidisciplinary research across glaciology and cryospheric science."
    url: "/research/"
    btn_label: "View Research"
    btn_class: "btn--primary"
  - image_path: https://placehold.co/400x300?text=People
    title: "People"
    excerpt: "Meet our faculty, researchers, and students conducting cutting-edge science."
    url: "/people/"
    btn_label: "View People"
    btn_class: "btn--primary"
  - image_path: https://placehold.co/400x300?text=Join+Us
    title: "Join Us"
    excerpt: "Explore opportunities for postdocs, students, and research fellows."
    url: "/join-us/"
    btn_label: "View Opportunities"
    btn_class: "btn--primary"
---

**Note:** This website is currently under production. Please bear with us whilst things get up and running! 
{: .notice--warning}


{% include feature_row %}

## About Us

The Bristol Glaciology Centre (BGC) focuses on the study of cold and ice-covered regions across the globe, from the Arctic to the Antarctic. Renowned for its multidisciplinary approach, the BGC employs advanced research methods, including remote sensing, numerical modeling, and field studies, to understand and address the impacts of changing cryospheric environments on ecosystems and communities.

The Centre comprises six faculty from the School of Geographical Sciences: Liz Bagshaw (Director), Jonathan Bamber, Tom Chudley, Stephen Cornford, Fabien Maussion (Director), and Chris Williamson. A number of Postdoctoral Research Associates and Fellows work with the faculty, mainly funded by grants from the UK Research Councils and the European Commission, together with Research Students supported by the UK research councils and the EU Marie Skłodowska-Curie Actions program. The Centre collaborates closely with other university groups, such as the Cabot Institute for the Environment, the Jean Golding Institute, and more.

The approach of Centre staff is broad in terms of both the scientific methods of investigation used and the geographical areas studied. Glaciological problems usually require multi-disciplinary solutions, and approaches using a combination of field investigation, remote sensing (from ships, aircraft and satellites), field and laboratory biogeochemical/microbiological measurements and numerical modelling are typical. Current studies are taking place on glaciers and larger ice masses from Antarctica to Greenland, Svalbard to the European Alps.

---

## Latest News

{% for post in site.posts limit:3 %}
  <div class="notice--info">
    <h4><a href="{{ post.url }}">{{ post.title }}</a></h4>
    <p><em>{{ post.date | date: "%B %d, %Y" }}</em></p>
    {{ post.excerpt }}
  </div>
{% endfor %}

[View all news →](/news/){: .btn .btn--primary}
