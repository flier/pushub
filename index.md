---
layout: page
title: Pushub.io
tagline: Connect and Learn your users, communicate with realtime Medias
carousel:
  id: myCarousel
  items:
    - 
      title: Connect 
      desc: Push message to the right customers and receive feedback from them, whether your mobile apps is running or offline, connect them over all the platforms (iOS, Android, Window Phone 7/8 and HTML/AJAX).
      img: slide-01.jpg
      action:
        name: Learn more
        url: features/connect.html
    - 
      title: Learn 
      desc: Know your users when, where and how to use your mobile apps, learn their use behaviors, and read realtime and analystic reports to identify your next customer and income.
      img: slide-02.jpg
      action: 
        name: Learn more
        url: features/learn.html
    - 
      title: Media 
      desc: Push and receive the realtime voice, video, photos and files from and to the users, redirect to your online customer services, or store in the cloud or your media servers.
      img: slide-03.jpg
      action: 
        name: Learn more
        url: features/medias.html

---
{% include JB/setup %}

<div class="row">
  {% for item in page.carousel.items %}
  <div class="span4">
    <h2>{{ item.title }}</h2>
    <p>{{ item.desc }}</p>
    <p><a class="btn" href="{{ item.action.url }}">{{ item.action.name }}</a></p>
  </div>
  {% endfor %}
</div>
