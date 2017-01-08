---
layout: post
title:  "Building erdemtu.com - Functionality & Technology"
date:   2017-01-08 20:07:34 +0300
categories:
---

Next step in building erdemtu.com is listing the features and deciding on
the technology to implement the functionality.
[My previous post](http://erdemtu.com/2016/12/28/building-erdemtu-com-purposes-functionality.html)
should be helpful.

### Features

- Create, edit, draft & publish blog posts.
    - Blog posts should have tags and categories.
- Create & edit portfolio items.
    - Portfolio items should have categories.
- Create & edit page items.
- Markdown editor for inputting content.
    - Should be able to upload images.
    - Should be able to migrate old content.
- Paths should be the same as Jekyll.
- Authentication for admin panel.
    - Should be able change password for the panel.
    - Should be able reset password with email.

That's it for the features. They cover most of the purposes I outlined earlier.
Should be enough of an exercise to begin with. Showing off part is the design
part.

### Technology

I am planning on using Vapor for backend. I already know Swift so I can focus on
learning backend stuff. Vapor is not that mature but it should be fine for such
a simple site.

For frontend I am considering React but Angular is tempting as well. I'll pick
React for now. Could be useful to know React, in case I wanted to learn React
Native.

### Next Steps

Next time I'll write about the design of site. A wireframing is the more
traditional route but with such simple site, I'll probably get on with the
design of each page.
