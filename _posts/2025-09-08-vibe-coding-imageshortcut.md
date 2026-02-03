---
title: "Vibe Coding ImageShortcut"
slug: "vibe-coding-imageshortcut"
description: |
  I decided to give "vibe coding" a try and it really works! It was like pair programming with a very experienced developer who has minor brain damage. I used ChatGPT 5 with assistance of Android Studio's Gemini bot.
  I started small by rebooting one of...
date: 2025-09-08
updated: 2025-09-08
status:
  - published
reading_time: 5
cover_image: "/assets/img/blog/2025-09-08-vibe-coding-imageshortcut/cover.png"
---
I decided to give "vibe coding" a try and it really works! It was like pair programming with a very experienced developer who has minor brain damage. I used ChatGPT 5 with assistance of Android Studio's Gemini bot.

I started small by rebooting one of my old Android apps which makes shortcuts on your launcher (home screen) to specific images in your gallery for easy access. Unlike widgets, shortcuts can be grouped together in folders.

The 0.2 version of this app dates back to 2011 and was hosted on [Google Code](https://code.google.com/archive/p/image-shortcut/). It targeted Android 2.3 Gingerbread and was written by hand.

Major improvements over the old version:

* [Shortcut api](https://developer.android.com/develop/ui/views/launch/shortcuts) (pinned shortcuts)
    
* [Photo Picker](https://developer.android.com/training/data-storage/shared/photo-picker) (no permissions required)
    
* It now copies the media to a private directory and cleans up orphans when shortcuts get removed.

In this first version, the shortcuts can only be created with a dedicated button but in the next versions I plan to bring back the *share from gallery* and widget style *create shortcut* features as well as cropping the shortcut's preview image. I'm not sure if the app should also support video files as these are often much bigger than images and keeping a copy would be inefficient.

[More Info Here](https://arnodenhond.com/imageshortcut)

---

I did have to give the A.I. some very specific instructions

* adaptive icon (otherwise the bitmap looks much worse)
    
* create the shortcut on the main ui thread

And I had to fix some strange errors

* missing imports
    
* broken gradle files

---

The app is free and has no ads. Get it on [Google Play](https://play.google.com/store/apps/details?id=arnodenhond.imageshortcut)

You can see the source code and planned improvements on [GitHub](https://www.github.com/arnodenhond/ImageShortcut)

If you decide to try it out, please post your use case as a rating to inspire others.
