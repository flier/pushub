---
layout: page
title: Hello World!
tagline: Supporting tagline
carousel:
  id: myCarousel
  items:
    - 
      title: Example headline.
      desc: Cras justo odio, dapibus ac facilisis in, egestas eget quam. Donec id elit non mi porta gravida at eget metus. Nullam id dolor id nibh ultricies vehicula ut id elit.
      img: slide-01.jpg
      action:
        name: Sign up today
        url: #
    - 
      title: Another example headline.
      desc: Cras justo odio, dapibus ac facilisis in, egestas eget quam. Donec id elit non mi porta gravida at eget metus. Nullam id dolor id nibh ultricies vehicula ut id elit.
      img: slide-02.jpg
      action: 
        name: Learn more
        url: #
    - 
      title: One more for good measure.
      desc: Cras justo odio, dapibus ac facilisis in, egestas eget quam. Donec id elit non mi porta gravida at eget metus. Nullam id dolor id nibh ultricies vehicula ut id elit.
      img: slide-03.jpg
      action: 
        name: Browse gallery
        url: #

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

Read [Jekyll Quick Start](http://jekyllbootstrap.com/usage/jekyll-quick-start.html)

Complete usage and documentation available at: [Jekyll Bootstrap](http://jekyllbootstrap.com)

## Update Author Attributes

In `_config.yml` remember to specify your own data:
    
    title : My Blog =)
    
    author :
      name : Name Lastname
      email : blah@email.test
      github : username
      twitter : username

The theme should reference these variables whenever needed.
    
## Sample Posts

This blog contains sample posts which help stage pages and blog data.
When you don't need the samples anymore just delete the `_posts/core-samples` folder.

    $ rm -rf _posts/core-samples

Here's a sample "posts list".

<ul class="posts">
  {% for post in site.posts %}
    <li><span>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ BASE_PATH }}{{ post.url }}">{{ post.title }}</a></li>
  {% endfor %}
</ul>

## To-Do

This theme is still unfinished. If you'd like to be added as a contributor, [please fork](http://github.com/plusjade/jekyll-bootstrap)!
We need to clean up the themes, make theme usage guides with theme-specific markup examples.
