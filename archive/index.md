---
layout: container-template
title: Archive
comments: false
---

<div class="row">
  <div class="col-lg-8 col-lg-offset-2 col-md-10 col-md-offset-1">
    <h3 class="center-block"><u>Archive</u></h3>
    
    <div class="archiveContainer">
      <ul>
        {% for post in site.posts %}
          <li>
            &nbsp;  {{ post.date | date_to_string }} &raquo; 
            <a href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a><br/>          
          </li>
        {% endfor %}
      </ul>
    </div>
  </div>
</div>