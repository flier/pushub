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

<style>

  /* GLOBAL STYLES
  -------------------------------------------------- */
  /* Padding below the footer and lighter body text */

  body {
    padding-bottom: 40px;
    color: #5a5a5a;
  }



  /* CUSTOMIZE THE NAVBAR
  -------------------------------------------------- */

  /* Special class on .container surrounding .navbar, used for positioning it into place. */
  .navbar-wrapper {
    position: absolute;
    top: 0;
    left: 0;
    right: 0;
    z-index: 10;
    margin-top: 20px;
    margin-bottom: -90px; /* Negative margin to pull up carousel. 90px is roughly margins and height of navbar. */
  }
  .navbar-wrapper .navbar {

  }

  /* Remove border and change up box shadow for more contrast */
  .navbar .navbar-inner {
    border: 0;
    -webkit-box-shadow: 0 2px 10px rgba(0,0,0,.25);
       -moz-box-shadow: 0 2px 10px rgba(0,0,0,.25);
            box-shadow: 0 2px 10px rgba(0,0,0,.25);
  }

  /* Downsize the brand/project name a bit */
  .navbar .brand {
    padding: 14px 20px 16px; /* Increase vertical padding to match navbar links */
    font-size: 16px;
    font-weight: bold;
    text-shadow: 0 -1px 0 rgba(0,0,0,.5);
  }

  /* Navbar links: increase padding for taller navbar */
  .navbar .nav > li > a {
    padding: 15px 20px;
  }

  /* Offset the responsive button for proper vertical alignment */
  .navbar .btn-navbar {
    margin-top: 10px;
  }


  /* RESPONSIVE CSS
  -------------------------------------------------- */

  @media (max-width: 979px) {

    .container.navbar-wrapper {
      margin-bottom: 0;
      width: auto;
    }
    .navbar-inner {
      border-radius: 0;
      margin: -20px 0;
    }
  }


  @media (max-width: 767px) {

    .navbar-inner {
      margin: -20px;
    }
  }
</style>

<div class="row">
  {% for item in page.carousel.items %}
  <div class="span4">
    <h2>{{ item.title }}</h2>
    <p>{{ item.desc }}</p>
    <p><a class="btn" href="{{ item.action.url }}">{{ item.action.name }}</a></p>
  </div>
  {% endfor %}
</div>
