---
layout: post
title:  "Emoji Subdomain"
date:   2023-02-22 23:29:15 -0800
# weather: 
# location: 
mood: 🦄
categories: tech
tags: IndieWeb Emoji Websites
---
So I made myself an emoji subdomain. It works, which is really fun. But I guess I need to add it to my certificate.

Given the option, why would I not use a 🦄 subdomain?

You can try going to my homepage at the alternate subdomain [🦄.shannonkay.com](https://🦄.shannonkay.com)

*Update: Here's how I set up the emoji subdomain.*

To create an emoji subdomain, you need to get the punycode for the emoji. (Note that the punycode is different from the [unicode](https://unicode.org/emoji/charts/full-emoji-list.html).) I used [Punycoder](https://www.punycoder.com) to get the punycode. Just paste the emoji you want to use into the "text" box, and click "convert to punycode". You can now copy the resulting punycode from the punycode box. 

The unicorn emoji 🦄 punycode is "xn--3s9h"(without the quotes).

Next, you can go to your domain registrar and create a subdomain. I use [Name.com](https://www.name.com).  When you create the subdomain, use the emoji's punycode where you want the emoji to go. (For me, making a subdomain meant going to "manage DNS" and creating a CNAME record with the subdomain pointing to my website). 

A subdomain is something like *unicorn.shannonkay.com*. To make it [🦄.shannonkay.com](https://🦄.shannonkay.com) instead, create the subdomain xn--3s9h.shannonkay.com. When I did this, the emoji showed up in the Manage DNS list for the subdomain as soon as I added the DNS record. 

To set the subdomain up with your hosting, add it to your your SSL certificate, etc. You'll need to use the punycode version of the subdomain. But once you've done that, you should be able to type the emoji version into your browser and link to it from most places. 

There are some downsides to the emoji subdomain. It's not good for email, and places like Instagram don't support using emoji in links. So it's probably best not to have emoji in your only linking option. 

### Links
- [Punycoder](https://www.punycoder.com) 
- [Emoji Finder](https://emojifinder.com)
- [Emojipedia](https://emojipedia.org) 
- [GetEmoji](https://getemoji.com)
- [Emoji Domain on Wikipedia](https://en.wikipedia.org/wiki/Emoji_domain)