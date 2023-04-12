---
layout: post
title:  "Reply By Email"
# subtitle: Each post also has a subtitle
date:   2023-04-11 23:11:00 -0800
# weather: 🌥️ 🔆 
# location: <a href="https://www.letitbrie.com">Let It Brie</a>
# mood: 🥰
# cover-img: /assets/img/path.jpg
# thumbnail-img: /assets/img/2023/LetitBrie.jpg
# share-img: /assets/img/2023/LetitBrie.jpg
categories: tech
comments: true
tags: [ email, reply, blog, Jekyll ]
---

I opened my RSS reeder to my newly formed folder of Personal Blog feeds and read a nice post on [Zinzy’s website](https://www.zinzy.website) about her puppy meeting a cat. I noticed that she has a “reply by email” link. It was just a normal mailto link to her email address. I made a short reply by email and thought that was a pretty nice way to comment.

I remembered that you can configure a subject for a mailto link, and thought about how I could set my Jekyll blog up to fill in a subject based on the blog post title.

I couldn’t quite remember the syntax for adding the subject to the mailto link, so I did a search. I found this nice [tool for creating mailto links](https://mailto.vercel.app). I added a prefix to the subject, and used the Jekyll templating for page title. I also used an iCloud “hide my” email address, to prevent my real email address from being scraped and spammed. 

```html
<a href="mailto:EMAIL@DOMAIN.COM?subject=%5BBlog%20Reply%5D%20{{ page.title }}">Reply by email</a>
```

I added the email link to the top of my comments html file. Now when you click on the “Reply by Email” link under my blog post, it will fill in the subject in with the title of the blog post you ‘re replying to. It's simple, but customized.