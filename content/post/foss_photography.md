+++
date = "2017-05-06T21:30:06-04:00"
description = "A brief introduction to some of the many great (and free!) resources for open source photo organizing and editing."
title = "Some Resources for Free Photography Software"

+++

<a href="https://www.flickr.com/photos/9bladed/33612284144/in/album-72157670803546106/" title=" Lizard"><img class="wide" src="https://c1.staticflickr.com/5/4156/33612284144_1567fc232e_o.jpg"></a>
*A lizard pauses for a photo I took last year on a rafting trip in the Grand Canyon.*
[[Flickr](https://www.flickr.com/photos/9bladed/33612284144/in/album-72157670803546106/), [500px](https://500px.com/photo/210567161/lizard-by-john)]

Whether you are a budding amateur or a seasoned professional photographer, the software tools you use play an important role in organizing, editing, and showing your photos. Maybe you are tired of continuing to pay Adobe as all their software moves to subscription or are looking for some of the best tools out there which also happen to be free. In this post I want to introduce some tools and resources for free (or libre) software that I use or can recommend.

By [free software](https://www.gnu.org/philosophy/free-sw.html) I mean programs that a user has the freedom to use and do with as they like, including looking at and modifying the underlying computer code. While most people using these applications won't ever do anything with the code, there are many benefits to anyone using it. The more active projects tend to develop quickly, with frequent changes, bug fixes, and overall responsiveness to the community. There is no chance the program can just disappear (the source code is available) and will continue to be supported as long as someone is willing to work on it. Finally, even if you do not have a strong belief in the principles of truly free software, there are some fantastic programs out there that compete with the expensive offerings from Adobe and the like...and it's free.

Before diving in, let me mention the website [Pixl.us](https://pixls.us/), dedicated to free and open source photography with a blog, in depth articles, and active [discussion forum](https://discuss.pixls.us/). Since I'll (mostly) be talking about programs I use regularly, take a look at their very nice [list of software](https://pixls.us/software/) for a more complete list.


## Calibration, Organizing, and Tagging

* [DisplayCAL (formerly dispcalGUI)](https://displaycal.net/)

is an excellent and advanced tool for calibrating displays with appropriate hardware tools, a must for anyone to accurately edit and display photos. It is much better than a lot of the basic manufacturer supplied software (which are often intentionally crippled), or tools builtin to an OS. DisplayCAL can be a bit overwhelming to use, though the documentation on the website is quite thorough. I just found [this quick start guide](https://www.pointsinfocus.com/learning/digital-darkroom/displaycal-and-argyll-cms-quick-start-guide/) that may help you get started.

* [gps4cam](http://gps4cam.com) (not open source and possibly no longer updated)

I use  to geotag (put GPS coordinates on photos). To use this tool in linux, follow [these simple steps](https://blog.andi95.de/2014/10/gps4cam-and-linux/).

I wrote a simple reverse geocoding (getting location name and other attributes from GPS coordinates) script, which you can find on [GitHub](https://github.com/podiki/reverse_geo). (This script also copies some tags written by Darktable into IPTC slots.)

The above script uses [ExifTool](http://www.sno.phy.queensu.ca/%257Ephil/exiftool/) for reading and writing information into photos, which is also used behind the scenes in many of the other tools mentioned. If you need to dig into a picture's metadata for any reason that is not covered by one of the other programs, you can just directly use ExifTool.

[Rapid Photo Downloader](http://www.damonlynch.net/rapid/) (Linux only) is a program for copying, moving, and renaming photos between the camera (SD cards, etc.) and your computer, or between drives.

[digiKam](https://www.digikam.org/) is an all in one photo manager and editor, but is especially noted for its organizational and tagging abilities.


## Post Processing

### Darktable
I started using Darktable at the end of last year as a replacement for Adobe's Lightroom, which I have used for many years. I would argue that Darktable is more advanced and capable than Lightroom in its editing capabilities, although less so for organizing (though it does okay there, too). Like any good (non-destructive) photo editing tool it can take some time to pick up, especially as there are many different modules, multiple ways of doing things, and many advanced features. The links I list below are very helpful, from just starting out to diving in deep to all that it can do.

All of the [photos](https://flic.kr/s/aHskKLsCay) in my [Paris photo essay](/photo-essay/paris) were edited entirely with Darkroom, learning as I went (and coming from a background in Lightroom). I have been very pleased with the results and continue finding new ways to improve my post processing in Darktable.

- [Darktable](https://darktable.org/)'s official website is where you can keep up with the latest releases. Their [resources page](https://www.darktable.org/resources/) has the very useful manual, as well as some older but still good links.
- [Film emulation presets](http://www.joaoalmeidaphotography.com/en/t3mujinpack-film-darktable/)
- On the [Pixl.us blog](https://pixls.us/blog/2017/02/from-the-community-vol-2/) highlighted this [discussion on grain](https://discuss.pixls.us/t/lets-improve-grain/2709) which [will be incorporated](https://github.com/darktable-org/darktable/pull/1386) in a future version (looks to be 2.4) of Darktable.

#### Videos
* [Riley Brandt's Darktable Tutorials](https://www.youtube.com/playlist?list=PL33t7emXCBHkMfiP1IcO-0_4mUAhh1lFA), see also his other videos like this one on [Darktable masks](https://www.youtube.com/watch?v=SKknBy5lX7I) of some [GIMP tutorials](https://www.youtube.com/playlist?list=PL33t7emXCBHlN4VnjHJaCyGqrTcGrLTUw)
* Harry Durgin's [Weekly Edit](http://weeklyedit.com/) [Darktable Edits playlist](https://www.youtube.com/playlist?list=PLsks-zRRM1ZVN_g7P6ZAsYVqTltmXyBjl)
* Robert Hutton's [Darktable videos](https://www.youtube.com/playlist?list=PLmvlUro_Up1NBX7VK8UUuyWo1B468zEA0)

## Other great options
A heralded RAW converter [RawTherapee](http://rawtherapee.com/)

Also digikam.

*The* open source image editing program, [GIMP](https://www.gimp.org/)

## Image viewing

[Geeqie](http://geeqie.org/) (Linux) a lightweight image viewer that is color profile aware.

[Firefox](https://www.mozilla.org/en-US/firefox/) is color managed, but you should [follow these instructions](http://cameratico.com/guides/firefox-color-management/). While [Google Chrome](https://www.google.com/chrome/) or [Chromium](https://www.chromium.org/Home) based browsers have [several](https://bugs.chromium.org/p/chromium/issues/detail?id=667433) [bugs](https://bugs.chromium.org/p/chromium/issues/detail?id=667431).

## Giving back

Submit bug reports, do some hacking, donate money.

Share your work with a [copyright (or copyleft license)](https://creativecommons.org/share-your-work/) from [Creative Commons](https://creativecommons.org/) and/or contribute images to [Wikimedia Commons](https://commons.wikimedia.org/wiki/Commons:Welcome) where they can be used for projects like [Wikipedia](https://www.wikipedia.org/).

## Workflow

Take a look at [Riley Brandt's open source photography workflow](https://www.rileybrandt.com/2015/10/15/foss-photo-flow-2015/); my own is very similar.

My basic workflow is this

1. card to computer
2. gps4cam
3. rapid downloader rename
4. darktable import
5. edit
6. export
7. run script
8. upload
9. test
10. ing
11. more
12. numbers
