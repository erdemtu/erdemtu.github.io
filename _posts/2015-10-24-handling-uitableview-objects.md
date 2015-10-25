---
layout: post
title:  "Handling UITableView Objects"
date:   2015-10-24 16:13:14 +0300
categories:
---

While developing for iOS, it is pretty much inevitable to work with `UITableView`
objects. They are pretty powerful and useful but handling tableviews with
multiple types of cells and updating their contents can be cumbersome.

For [Socialeyes](https://itunes.apple.com/app/id550806403?) and [Kahve Falmania](https://itunes.apple.com/au/app/kahve-falmania/id536516340?mt=8) I
developed my own table manager; Instead of feeding separate information about
the same row via multiple functions and protocols, I model the whole tableview
in one go, and update it with function.

The result considerably sped up my workflow with table views but I was reluctant
to share my TableViewManager; Having built it, I knew very well how to use it
but I suspected it was too much custom tailored for myself. I was too busy to
refine and document it for others so I kept on postponing it.

Now that I am working with Swift, I am also porting my TableViewManager
to Swift as an exercise and to make it simpler. Swift is certainly simplifying the
library though for now It is not as "Swifty" as I want. Maybe there are some
classes that can be made into protocols or structs instead. Maybe generics can
make constructing tableview models safer. I'll try to keep my eyes open for
those kinds of opportunities.

In the mean time, I came across other "TableViewManager" libraries:
[RETableViewManager](https://github.com/romaonthego/RETableViewManager),
[DTTableViewManager](https://github.com/DenHeadless/DTTableViewManager) and
[Static](https://github.com/venmo/Static). They seem to be popular so I'll
be sure to investigate their take on the problem.

Lastly I think with iOS 9 `UIStackView` looks like it could handle some cases
where it was easier to use a `UITableView` before.
