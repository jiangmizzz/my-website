---
layout: single
title: "My first post"
# classes: wide
categories: [Daily records]
tag: [Development, Website]
toc: true
toc_label: "My first post"
toc_icon: "paw"  # corresponding Font Awesome icon name (without fa prefix)
toc_sticky: true
---
Welcome, this is my first post on my personal website! And I will share some insights I gained during the website building process.
--> [Github repository](https://github.com/jiangmizzz/my-website)

## Overview
I seleceted [Mimimal Mistake](https://mmistakes.github.io/minimal-mistakes/) to build the first darft of my website because I really want to have a personal website equipped with blog function and can be customized.

When starting my work, I also took the [academicpages](https://github.com/academicpages/academicpages.github.io), [al-folio](https://github.com/alshedivat/al-folio) and other highly complete templates into my consideration. And after my exploration and practice, I think it might be a much easier way to use them:D, although they didn't quite meet my needs in some aspects. I encountered amounts of obstacles in this process, which I will mention below.

## Details & Insights
### Install Jekyll on MacOS
This is the first barrier I encountered. MacOS does not support installing Jekyll directly, otherwise you'll suffer from the trouble of installation failure and error `jekyll: command not found`.

To solve this problem, I tried to search the answer on Stack Overflow and have asked genAI for many times, but it didn't work. Finally, I refered to this [official guidance](https://jekyllrb.com/docs/installation/macos/) and successfully solved the problem by installing the `chruby`. It was really helpful.

A successful installation is indicated by entering the following command in the terminal and then seeing `jekyll x.x.x` as the output:
```terminal
$ jekyll -v 
```

### Manage my Publications & News
Since the Minimal Mistake does not provide publications and news templates, and this two parts are usually vital in academic pages. I needed to write and add them manually. That's why I mentioned abovet that it can be much easier to use other academic templates with ready-made templates of this type. But I had made my decision and honestly perferred the current page style, so it was my responsibility to overcome this problem XD.

As you can see now, I have successfully added these two sections to my webpage. The process was a bit tricky, and I went through many trials and errors to figure out their compatibility with the original template (Of course, I don't want to add them like patches). If anyone have the same requirement with me, I recommend that you refer to this part of the style in other academic templates for your design or to adapt it (it's usually located in the `_includes` folder). For me, I referenced [this template](https://github.com/domoritz/domoritz.github.io/tree/master) and made some personal adjustments to complete the design of the publications section, and designed the news list on my own.

It was not a very simple matter though, because it requires you to learn the basic Liquid grammar and modify them in the file. So for those who are in strong need of this two parts (publications and news list) and not very desired to learn the specific code files, it might be better to choose another website template (orz). Alternatively, you can modify my template according to your own needs and use it directly (It is still not a very nice template though). I would be very grateful for your appreciation ❤️.


### Breadcrumb
*To be added* 
-- This problem happened when I wanted to set a convenient archive system for my posts. Although the problem is solved, I still don't understand why it occurred...
{: .notice}

### Favicon
Actually, the official docs does not contain the tutorial on setting up a favicon. But it is quite easy. Just enter the `/_includes/head/custom.html` and add a line of code like this: 
```html
 <link rel="icon" type="image/png" href="{{ '/assets/images/cat.png' | relative_url }}">
 ```
I drew a icon by myself, which is a cow cat. Although it does not very detailed but cute, isn't it?
![My cat](/assets/images/cat.png){: .align-center width="50%"}
 *🐱 — a black and white cutie who looks like a tiny cow!* 


## Future plan
I currently use the [dirt theme](https://mmistakes.github.io/minimal-mistakes/docs/configuration/#dirt-skin-dirt) provided by the template, which is a soft and pleasant theme. And as the next step, I plan to deisgn and apply my own color theme to this website. Since <span class="first-post-green-text">green</span> is my favorite, I suppose it will be the primary color of my next website skin.