+++
title = "Some Resources for Free Photography Software"
description = "A brief introduction to some of the many great resources for free software for photographers."
date = "2017-05-17T15:30:00-04:00"
categories = [ "Blogpost" ]
tags = [ "Photography", "Free Software", "Open Source" ]
image = "https://c1.staticflickr.com/5/4156/33612284144_1567fc232e_o.jpg"
imagecap = "A lizard pauses for a photo I took last year on a rafting trip in the Grand Canyon. [[Flickr](https://www.flickr.com/photos/9bladed/33612284144/in/album-72157670803546106/), [500px](https://500px.com/photo/210567161/lizard-by-john)]"
imagelink = "https://www.flickr.com/photos/9bladed/33612284144/in/album-72157670803546106/"
+++

Whether you are a budding amateur or a seasoned professional photographer, the software tools you use play an important role in organizing, editing, and showing your photos. Maybe you are tired of continuing to pay Adobe as all their software moves to subscriptions or are looking for some of the best tools out there which also happen to be free. In this post I will introduce some free (or "libre") software and related resources that I use or can recommend.

<!--more-->

By [free software](https://www.gnu.org/philosophy/free-sw.html) I mean programs that a user has the freedom to use and do with as they like, including looking at and modifying the underlying computer code. While most people using these applications won't ever do anything with the code, there are many benefits to anyone using it. The more active projects tend to develop quickly, with frequent changes, bug fixes, and overall responsiveness to the community. There is no chance the program can just disappear (the source code is available) and it will continue to be supported as long as someone is willing to work on it. Finally, even if you do not have a strong belief in the principles of truly free software, there are some fantastic programs out there that compete with the expensive offerings from Adobe and the like...and are free.

Before diving in, let me mention the excellent website [Pixl.us](https://pixls.us/), dedicated to free and open source photography with a blog, in depth articles, and active [discussion forum](https://discuss.pixls.us/). Since I'll (mostly) be talking about programs I use regularly, take a look at their very nice [list of software](https://pixls.us/software/) for a more complete list.


### Calibration, Organizing, and Tagging

Here are some helpful programs for getting started with your open source photography workflow, from calibrating your monitor to geotagging photos.

##### [DisplayCAL](https://displaycal.net/)
DisplayCAL (formerly dispcalGUI) is an excellent and advanced tool for calibrating displays with appropriate hardware tools, a must for accurately editing and displaying photos. It is much better than a lot of the basic manufacturer supplied software (which are often intentionally crippled), or tools built into an operating system (OS). DisplayCAL can be a bit overwhelming to use, though the documentation on the website is quite thorough. I just found [this quick start guide](https://www.pointsinfocus.com/learning/digital-darkroom/displaycal-and-argyll-cms-quick-start-guide/) that may help you get started. Make sure that the resulting color profile is loaded and used by any program that can (like the editing and viewing ones noted below).

##### [gps4cam](http://gps4cam.com)
I use gps4cam for geotagging photos (saving location information): you use their app on a smartphone to log GPS coordinates, and then their computer application to write this information to your photos. To use this tool in Linux, follow [these simple steps](https://blog.andi95.de/2014/10/gps4cam-and-linux/). *Note:* Not open source and possibly no longer updated.

##### [Rapid Photo Downloader](http://www.damonlynch.net/rapid/) (Linux only)
This program is good for copying, moving, and renaming photos between the camera (SD cards, etc.) and your computer, or between drives.

##### [digiKam](https://www.digikam.org/)
digiKam is a comprehensive photo manager and editor, but is especially noted for its organizational and tagging abilities.

##### [Simple reverse geocoding script](https://github.com/podiki/reverse_geo)
I wrote a simple reverse geocoding (getting location name and other attributes from GPS coordinates) script using Python and other free tools. Given photos with GPS coordinates, it will write country, region, and city information to a new copy of the file. (This script also copies some tags written by Darktable into IPTC slots.)

##### [ExifTool](http://www.sno.phy.queensu.ca/%257Ephil/exiftool/)
The above script uses ExifTool for reading and writing information into photos, which is also used behind the scenes in many of the other tools mentioned. If you need to dig into a picture's metadata for any reason that is not covered by one of the other programs, you can just directly use ExifTool.


### Post Processing

This is where you'll be spending most of your time, and, as it turns out, where the free software offerings are every bit as good (or better) than commercial options. I will be highlighting Darktable as that is what I have been using, but there are some other options I will mention as well.

#### Darktable
I started using [Darktable](https://darktable.org/) at the end of last year as a replacement for Adobe's Lightroom, which I have used for many years. I would argue that Darktable is more advanced and capable than Lightroom in its editing capabilities, although less so for organizing (but it does okay there, too). Like any good (non-destructive) photo editing tool it can take some time to pick up, especially as there are many different modules, multiple ways of doing things, and many advanced features. The links I list below I've found to be very helpful, from just starting out to diving in deep to all Darktable can do.

All of the [photos](https://flic.kr/s/aHskKLsCay) in my [Paris photo essay](/photo-essay/paris) were edited entirely with Darkroom, learning as I went (and coming from a background in Lightroom). I have been very pleased with the results and continue finding new ways to improve my post processing in Darktable.

* [Darktable](https://darktable.org/)'s official website is where you can keep up with the latest releases.
* The official [resources page](https://www.darktable.org/resources/) has the very useful manual, as well as some older (but still useful) links.
* The [forum on Pixl.us](https://discuss.pixls.us/c/software/darktable) is a pretty active place to discuss Darktable.
* Darktable let's you save post processing settings as a preset for quickly duplicating a particular style later on. There is a huge repository of them available on [dtsyle](https://dtstyle.net/).
* João Almeida has made an extensive collection of [film emulation presets](http://www.joaoalmeidaphotography.com/en/t3mujinpack-film-darktable/), bringing the look of your favorite black and white, color, or slide film for easy use in Darktable.
* To check if color profiles are being correctly used by Darktable, run `darktable-cmstest` from a terminal. [This page of the documentation](https://www.darktable.org/usermanual/ch03s02s10.html.php) has more about color management in Darktable.
* The [Pixl.us blog](https://pixls.us/blog/2017/02/from-the-community-vol-2/) highlighted this [discussion on improving grain](https://discuss.pixls.us/t/lets-improve-grain/2709) which [will be incorporated](https://github.com/darktable-org/darktable/pull/1386) in a future version (slated for 2.4) of Darktable. This is a great example of the power of free and open source software and an active community.

##### Videos
* [Riley Brandt's Darktable Tutorials](https://www.youtube.com/playlist?list=PL33t7emXCBHkMfiP1IcO-0_4mUAhh1lFA) is an excellent starting point. See also his other videos like this one on [Darktable masks](https://www.youtube.com/watch?v=SKknBy5lX7I) (a killer feature which allows you to use nearly any editing module in a local area and/or by user defined parameters) or his [GIMP tutorials](https://www.youtube.com/playlist?list=PL33t7emXCBHlN4VnjHJaCyGqrTcGrLTUw). He also has a course on open source photography, but I have no experience with that.
* Harry Durgin's [Weekly Edit](http://weeklyedit.com/) (or [Darktable Edits playlist](https://www.youtube.com/playlist?list=PLsks-zRRM1ZVN_g7P6ZAsYVqTltmXyBjl) on YouTube) is an ongoing in-depth video series on advanced Darktable post processing. There are countless tricks and techniques in these videos that will take anyone's Darktable skills to another level.
* Robert Hutton's [Darktable videos](https://www.youtube.com/playlist?list=PLmvlUro_Up1NBX7VK8UUuyWo1B468zEA0) are a bit older (and sadly nothing new for quite a while), but there is an extensive set of videos here to dive into.


#### Other great options
##### [RawTherapee](http://rawtherapee.com/)
RawTherapee has a heralded raw converter and is a very well regarded post processing program. While I have yet to try it myself, I have heard many good things and it is another popular option. And take a look at [RawPedia](http://rawpedia.rawtherapee.com/Main_Page), their excellent encyclopedia for RawTherapee and everything raw related.

##### [digiKam](https://www.digikam.org/)
The aforementioned digiKam is also a capable application for post processing, giving you an all-in-one stop for organizing, editing, and exporting photos.

##### [GIMP](https://www.gimp.org/)
And, of course, there is *the* open source image editing program, the GIMP. This is the free software equivalent of Photoshop, with all the depth and complexity that entails. I have not used it for any real photo editing so far, but since it is very popular it should be easy to find a wealth of resources online to learn it.


### Image viewing

While you will likely have an image viewer with your OS, if you want to view photos with proper color management you have to look into the details. Many OSes do some form of color management, but there is plenty of variation in how effective they are and what programs will utilize this. Color profiles and management are becoming more of an issue these days as larger gamut (more colorful) displays are no longer relegated to the realm of expensive equipment for professionals. Without proper calibration (see earlier in the post) and color management, colors will look very different than they are supposed to. Most commonly on newer displays with wider color spaces images will look much more colorful and saturated (easily over saturated) without color management. This is a huge, and hugely confusing, topic outside the scope of this post, but here are few tips for basic image viewing.

##### [Geeqie](http://geeqie.org/) (Linux only)
Geeqie is a lightweight and easy to use image viewer that is color profile aware.

#### Browsers
[This article](http://cameratico.com/guides/web-browser-color-management-guide/) is a nice overview of color management in browsers (and in general). The upshot is that if you want to have proper colors in a browser, using ([a properly configured](http://cameratico.com/guides/firefox-color-management/)) [Firefox](https://www.mozilla.org/en-US/firefox/) is your best bet. Thankfully, there does seem to be some improvements across the board in supporting color management, although change has been very slow and it is often neglected. For example, [Google Chrome](https://www.google.com/chrome/) and [Chromium](https://www.chromium.org/Home) based browsers have [several](https://bugs.chromium.org/p/chromium/issues/detail?id=667433) related [bugs](https://bugs.chromium.org/p/chromium/issues/detail?id=667431), but are finally moving in the right direction.


### Workflow

As an example of how these applications work together and what a free software photography workflow might look like, here is an overview of how I have been doing it lately (and, of course, I'm constantly tweaking). Also take a look at [Riley Brandt's open source photography workflow](https://www.rileybrandt.com/2015/10/15/foss-photo-flow-2015/); my own is very similar:

1. Transfer photos from SD card to computer (in a temporary folder)
2. Use gps4cam to geotag
3. Use Rapid Photo Downloader to move and rename photos into final folder structure
4. Backup! (often I do this later, but never delete of off SD cards until backed up)
5. Import into Darktable
6. Make selections and post process in Darktable
7. Export final jpeg from Darktable
8. Run my reverse geocoding and tag cleanup script
9. Upload to [Flickr](https://www.flickr.com/9bladed), [500px](https://500px.com/9bladed), etc.

A common workflow I've seen is to use digiKam for organizing and tagging, and either staying in digikam for editing, or switching over to Darktable or RawTherapee. (*Note*: you can use XMP files for synchronizing things like tags between programs, but be sure that these are kept up to date and exported/re-imported as needed.) There are many good options to find exactly what fits your own needs and style.


### Giving back

Finally, a big ***thank you*** to everyone how has helped make all the fantastic free and open source programs listed in this article. It is truly remarkable the amount of time and effort that goes into something that is "given away."

On that note, we should all try to give back to these projects. Every little thing, from submitting bug reports, to doing some hacking, donating money, spreading the word, and so on, helps keep these projects alive and thriving. Take a look at their websites to see what you can do to help them out.

And when it comes to the photos themselves, you can share your work with a [copyright (or copyleft) license](https://creativecommons.org/share-your-work/) from [Creative Commons](https://creativecommons.org/) and/or contribute images to [Wikimedia Commons](https://commons.wikimedia.org/wiki/Commons:Welcome) where they can be used for projects like [Wikipedia](https://www.wikipedia.org/). There is also a [database of raw files](https://raw.pixls.us/) (recently [relaunched](https://pixls.us/blog/2017/01/new-year-new-raw-samples-website/)) from different cameras you can contribute to to help software developers and others.

I hope this article helps others to discover and flourish in the world of free and open source photography software. There's a lot more beyond what I've written here, so please feel free to leave a comment recommending your own favorite pieces of software or related resources.
