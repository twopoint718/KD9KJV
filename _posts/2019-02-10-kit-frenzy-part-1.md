---
layout: post
title:  "Kit Frenzy Part 1: GPS"
date:   2019-02-10 15:00:00 -0500
---

I picked up a few kits from QRP Labs and have been building them over the past few days. I just finished up the relatively-quick build for the QLG1, a standalone GPS receiver and clock source.

It may or may not be common knowledge that GPS satellites have the ability to provide very accurate time signals. It’s advertised that this will typically be within 40ns of the true value.

I plugged in the receiver and connected to it from my laptop via a USB/Serial connector. Here’s what I got:

<figure>
    <video style="width: 100%" controls src="https://s3.amazonaws.com/kd9kjv/video/gps.mov"></video>
    <figcaption>GPS serial data flying by</figcaption>
</figure>

Here’s what a line looks like:

```
$GPGGA,212759.000,4304.2770,N,08925.9501,W,2,8,1.06,281.5,M,-34.2,M,0000,0000*64
```

I looked it up and this is a data format known as NMEA.
Here’s a brief overview "$" starts a message, comma (",") is the delimiter.
After that the "GP" indicates that we’re talking to the US-based GPS system.
The next three letters indicate the type of message.
A "GGA" message is a location fix.
The fields are, in order:


- **212759.000** UTC time string, e.g. 21:27:59.000
- **4304.2770** decimal latitude, e.g. 43.042770
- **N** north of the equator
- **08925.9501** decimal longitude, e.g. 89.259501
- **W** west of the prime meridian
- **2** fix quality (2 = DGPS fix)
- **8** number of satellites used in this fix
- **1.06** horizontal dilution of position
- **281.5** altitude above sea level
- **M** (in meters)
- **-34.2** height of geoid at this position (as it differs from WGS84)
- **M** (in meters)
- **0000** empty field
- **0000\*64** empty field, then checksum (*64)

It’ll be fun to use this with the other kit that I got (the QCX transceiver) and maybe in other projects that need a little serial GPS data.
