---
layout: post
title:  "IndieWeb Bio ID Card"
# subtitle: Each post also has a subtitle
date:   2023-03-27 23:15:00 -0800
# weather: 🌥️ 🔆 
# location: <a href="https://www.letitbrie.com">Let It Brie</a>
# mood: 🥰
# cover-img: /assets/img/path.jpg
# thumbnail-img: /assets/img/2023/LetitBrie.jpg
# share-img: /assets/img/2023/LetitBrie.jpg
categories: tech
comments: true
tags: [html, css, microformats, IndieWeb ]
---

When I joined the [Indieweb Webring](https://🕸💍.ws/) on my [Homepage](https://www.shannonkay.com), I saw that it was looking for an h-card to make my profile. 

It said this:
> We'll look for your name, photo, and note on the [representative h-card](http://microformats.org/wiki/representative-h-card-authoring) on your page. If you're having trouble, you can [test your page with indiewebify.me](https://indiewebify.me/validate-h-card/?url=https://www.shannonkay.com/).


Suddenly I'm down a microformats IndieWeb rabbit hole, and have so much more to discover!

h-card html
```html
<section class="bio">
<span class="h-card">
<img class="u-photo" src="MYPHOTO.jpg" >
 <p><a href="MYWEBSITE" class="u-url u-uid p-name">MY NAME</a></p>
<p class="p-note">
My short bio text.
</p>
<p><abbr class="p-region" title="STATE">ST</abbr> - <a rel="me" href="MASTODON LINK" class="u-url">Mastodon</i></a></p>

</span>
</section>
```

h-card bio css
```css
.bio {
    background-color: #ffffff;
    border: 1pt solid #484848;
    border-radius: 10pt;
    width: 400px;
    margin-right: auto;
    margin-left: auto;
    text-align: left;
}

.bio img {
    float: left;
    margin: 5pt;
    border-radius: 5pt;
    max-width: auto; 
    max-height: 200px;
}
```

