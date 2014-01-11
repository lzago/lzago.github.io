---
layout: post
title: "OGRE video plugin"
date: 2014-01-11 21:48:25 +0000
comments: true
categories: [Ogre, DirectX, Game Programming]
---

It’s always a very common request in my daily gaming life to include HD, even FullHD videos in games, fullscreen videos, or even in-game videos. Even if i love Unity3D i must admit it has a very bad video management system. Unfortunately it supports only Theora format and at lower resolution than what i need (which is not actually hardware-accelerated).To support a decent hardware acceleration i had to rely on Directshow, which has the nice side effect to makes me delegate the decoding to the video decoders registered on the system, and to support more than one codecs. I used OGRE in the past, i really like the abstract approach it has to game programming letting you expand and maintain your games easily. So I noticed it had a Directshow video texture plugin, i thought of having solved the problem with that, unfortunately as soon as i tried it i realized that it was for a very old version of the engine, and with different bugs in it especially about memory management. So  i resurrected it   i made it working for OGRE 1.8.1. and fixed it in some points, here the download link, if you want to try it, VS2010 version.

[Download Here.](http://dl.dropbox.com/u/28836804/ogre_directshow.zip)

It works respecting the OGRE conventions, so setting OGRE_HOME and using the video as a material, you can have a video as Texture everywhere in your game. It works only in Windows, since Directshow is not portable.

It worked perfectly for my Lynx game, you could admire this summer, on London cinemas!

[Here](http://www.ogre3d.org/forums/viewtopic.php?f=4&t=37929&start=25) it’s the OGRE original forum thread where the plugin was discussed:

let me know if you found some problems using it. enjoy it.