---
layout: page
title: Material Pakistan
description: A live wallpaper app to show the astonishing monuments of Pakistan
img: assets/img/mp_splash_image.jpg
importance: 2
category: fun
---

<!-- Material Pakistan -->

A live wallpaper app to show the astonishing monuments of Pakistan

## About
Ever since we were young we saw that there was very little Pakistani content in the digital world. So we embarked on this journey to create as much content as we can in our free time!


### There are five variants of each six monuments which change with time

### Morning

<p align="center"> <img src="assets/img/mp/quaid_morning.jpg" width="180" height="300"> <img src="assets/img/mp/minare_pak_morning.jpg" width="180" height="300"> <img src="assets/img/mp/monument_morning.jpg" width="180" height="300"> </p>

### Afternoon

<p align="center"> <img src="assets/img/mp/quaid_afternoon.jpg" width="180" height="300"> <img src="assets/img/mp/minare_pak_afternoon.jpg" width="180" height="300"> <img src="assets/img/mp/monument_afternoon.jpg" width="180" height="300"> </p>

### Evening

<p align="center"> <img src="assets/img/mp/quaid_evening.jpg" width="180" height="300"> <img src="assets/img/mp/minare_pak_evening.jpg" width="180" height="300"> <img src="assets/img/mp/monument_evening.jpg" width="180" height="300"> </p>

### Night

<p align="center"> <img src="assets/img/mp/quaid_night.jpg" width="180" height="300"> <img src="assets/img/mp/minare_pak_night.jpg" width="180" height="300"> <img src="assets/img/mp/monument_night.jpg" width="180" height="300"> </p>

### Night (dark version)

<p align="center"> <img src="assets/img/mp/quaid_night_black.jpg" width="180" height="300"> <img src="assets/img/mp/minare_pak_night_black.jpg" width="180" height="300"> <img src="assets/img/mp/monument_night_black.jpg" width="180" height="300"> </p>


### All of the wallpapers were designed by <a href="https://www.linkedin.com/in/imsalmanafzal/">Salman Afzal</a>.


<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/1.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/3.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/5.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Caption photos easily. On the left, a road goes through a tunnel. Middle, leaves artistically fall in a hipster photoshoot. Right, in another hipster photoshoot, a lumberjack grasps a handful of pine needles.
</div>
<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/5.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    This image can also have a caption. It's like magic.
</div>

You can also put regular text between your rows of images.
Say you wanted to write a little bit about your project before you posted the rest of the images.
You describe how you toiled, sweated, _bled_ for your project, and then... you reveal its glory in the next row of images.

<div class="row justify-content-sm-center">
    <div class="col-sm-8 mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/6.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm-4 mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/11.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    You can also have artistically styled 2/3 + 1/3 images, like these.
</div>

The code is simple.
Just wrap your images with `<div class="col-sm">` and place them inside `<div class="row">` (read more about the <a href="https://getbootstrap.com/docs/4.4/layout/grid/">Bootstrap Grid</a> system).
To make images responsive, add `img-fluid` class to each; for rounded corners and shadows use `rounded` and `z-depth-1` classes.
Here's the code for the last row of images above:

{% raw %}

```html
<div class="row justify-content-sm-center">
  <div class="col-sm-8 mt-3 mt-md-0">
    {% include figure.liquid path="assets/img/6.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
  </div>
  <div class="col-sm-4 mt-3 mt-md-0">
    {% include figure.liquid path="assets/img/11.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
  </div>
</div>
```

{% endraw %}
