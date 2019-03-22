---
layout: post
title:  "Kit Frenzy Part 2: QCX"
---

The QCX is another [QRP Labs kit](https://qrp-labs.com/qcx.html).
This one was a trickier to build and took a lot longer.

<figure>
    <video style="width: 100%" controls src="https://s3.amazonaws.com/kd9kjv/video/wspr.mov"></video>
    <figcaption>QCX (all finished, but with the case opened up) running WSPR mode</figcaption>
</figure>

Sorry for the mostly image dump, but the photos show the progression of building the kit.
It took me about a week with a few days in there where I put in a good number of hours.
I am not a fast solder-er or part-picker.
But after this, I feel like I'm getting there.
Partway through I took the plunge of getting a binocular microscope and that turned out to be an amazing help.

<div class="gallery-wrapper">
{% assign thumbnails = site.static_files | where: "qcx-thumb", true %}
{% for thumbnail in thumbnails %}
  <a class="gallery-item" href="{{site.baseurl}}{{thumbnail.path | replace: "/thumbs", ""}}">
    <img src="{{site.baseurl}}{{thumbnail.path}}" />
  </a>
{% endfor %}
</div>

Winding toroids were the single most time-consuming part for me to work on.
For the first toroid, it was 3 windings of 3 turns and then 1 winding of 30 turns (I got the 20m version).
That winding process itself took me an hour or two.
I was a little nervous about getting it right though, and so I counted and inspected very carefully while I went.

The kit worked perfectly the first time I powered it up.
It includes some self-test equipment to help you calibrate the radio.
This led me to wonder what I/Q was.
And so I learned about [I/Q](http://whiteboard.ping.se/SDR/IQ) measurement -- well, not really, but now I know that there is something I should read up on.

I was able to hear plenty of CW stations right away just using a dipole that I put in my attic.
I've since built a lighter antenna with stranded wire of a lighter gauge (something like 16).
It's a small change in materials, but the antenna is a lot more portable and easy to work with.
