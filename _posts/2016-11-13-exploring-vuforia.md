---
layout: post
title:  "Exploring Vuforia"
date:   2016-11-13 14:45:02 +0300
categories:
---

I needed to use some augmented reality tech for a new iOS project. Basically
what I needed was some image targeting stuff; I needed to put an image, video or
a model on top of a predefined image in the screen. This has been possible for
years but hasn't been all that popular.

After some research I decided that Vuforia fit the bill. A few years ago I did
check out some of their samples. Back then it was called QCAR (good call on the
name change, I had to look up the old name to remember it).

Deciding how to use Vuforia was another process altogether. Vuforia has an SDK
for Objective-C, and another for Unity that I could use.

Objective-C SDK has the advantage of being used right in XCode. I could even use
it along with Swift and make use of my experiences in Cocoa Framework.
Unfortunately, apart from their own sample code, there is little activity in the
open. I found some sample code for [Swift & Scenekit](https://github.com/yshrkt/VuforiaSampleSwift)
but the way thing is setup doesn't allow more than one image to be targeted.
The transform matrices supplied by the SDK was used to tranform the position of
the camera in the scene, instead of the trackable object. I felt that despite
the SDK supplying me with the basic tools to handle the problem, it would take
me a lot of time to optimize the process. I could do a wrapper for Vuforia in
Swift in future but for now I decided to check out the Unity option.

With Unity things are very easy to setup. There is prefabs for trackable objects
and ARCamera, so it very simple to create a scene for the AR aspects of the app.
It is cumbersome to export the project to XCode & compile it, but it might be
worth it. Unity also has the advantage of being cross-platform, which might help
in the future. I've been meaning to use Unity for sometime which is another plus
.

I suspect setting up the UI for the rest of the app, won't be that pleasant in
Unity. Cocoa is not the easiest framework for setting up your UI but it is also
the framework I am most familiar with. I expect to be frustrated with Unity but
we'll see how it pans out. Worst case scenario, I'll write a Swift wrapper for
Vuforia and handle it all in XCode.     
