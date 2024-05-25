---
layout: post
title: Use Photos in GoodReads Reviews
date: 2024-05-24 23:15:14 -0800
categories: books tech
comments: true
tags:
---
Did you know that you can put photos in your GoodReads reviews? If you're a "bookstagrammer" and also use GoodReads, adding one(or more!) of your photos to a review can let even more book lovers enjoy them. 

Here's how to do it.

Upload your photo to an image host. Some choices include [Postimages](https://postimages.org), [imgur](https://imgur.com), and [Flickr](https://www.flickr.com). I normally use [SmugMug](https://www.smugmug.com) because I have a paid account there for my photos, and embedding is allowed. I'll use [Postimages](https://postimages.org) for this example.

After uploading your photo, copy the direct link to the image. GoodReads allows some  [HTML](https://developer.mozilla.org/en-US/docs/Web/HTML) formatting in reviews and we can use that to add a picture. 

Here is the HTML you need to embed the photo. Replace the LINK TO IMAGE with the direct link, and put in your own alt text. 

`<img src="LINK TO IMAGE" alt="BRIEF DESCRIPTION OF YOUR PICTURE" />`

Here's what mine looks like.

`<img src="https://i.postimg.cc/76jG8W1R/20231010-11-06-05.jpg" alt="Percy Jackson and the Chalice of the Gods on a table next to a pink mug" />`

Paste this code into your review on GoodReads, and save it. You can also click on "preview" to see what it looks like before you save. Paste the code wherever you want it to show up in the review. It could be at the beginning, at the end, or somewhere in the middle. It's up to you.

[Here's my review with the photo embedded](https://www.goodreads.com/review/show/5220271270).

These are the formatting tips from the GoodReads review editor. This tells us which HTML tags are supported. Notice that you can also include links. You could link to your blog, Instagram account, or even the direct link to a specific Instagram post. 
```HTML
Goodreads allows some html formatting.

well formed web urls automatically get turned into links
link: <a href="https://www.goodreads.com">my link text</a>
link to book: use the "add book/author" link or [book: The Hitchhiker's Guide to the Galaxy]
link to author: use the "add book/author" link or [author: J.K. Rowling]
image: <img src="https://www.goodreads.com/image..." width="40" height="100" alt="description"/> (Width must be 0-400, Height must be 0-1000, alt is a description of the image. All three are optional, but recommended.)
bold text: <b>...</b>
italic text: <i>...</i>
underline text: <u>...</u>
strike text: <s>...</s>
exact spacing: <pre>...</pre>
blockquote: <blockquote>...</blockquote>
paragraph: <p>...</p>
spoiler: <spoiler>...</spoiler>

Note: tags must be properly nested, example:
OK <i><b>test</b></i>
Not OK <i><b>test</i></b>
```

Enjoy!
