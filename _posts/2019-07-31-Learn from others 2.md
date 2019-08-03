---
layout: post
title: Learn from Apple/Google | Apple/Google로 부터 배우기
---

From the previous story, <br>
I have been writing errors which I have found from other map service providers. <br>
Most likely Apple and Google.
<br>
<br>
<br>
Before I start to write this article, <br>
I am not blaming employees at Apple and Google though you are going to see their mistakes.
<br>
<br>
<br>
Long story short, Apple still needs to improve their maps. (so does Google..)<br>
<br>
And from their mistakes, I have learned how to make/layer/design maps more<br>
At least,  I'm trying not to make same mistakes they made.<br>
For certain areas, my map is better than theirs. <br>
<br>
<br>
<br>
Again, don't get me wrong. I love Apple products and devices with Google services<br>
<br>
<br>
<br>
I database-nized all these just because I habe been making/designing/layering/analyzing maps for my work.
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
**Balance and harmony.**
<br>
<br>
I can't emphasize enough on the importance of them. <br>
Well trained cartographers should consider **balance and harmony** when they make maps. <br>
Especially, for map services, they become more important, for maps should satisfy all audiences.
<br>
<br>
<br>
I believe Apple Maps and Google Maps are well balanced.(except POIs. I have more things to say about POIs but it will come to next articles).<br>
Yet, there are some eyesoars.<.br>
Their data and layering orders make me somewhat uncomfortable.
<br>
<br>
<br>
**Let's start with pedestrian overpass.**
<br>
<br>
One day, I took a bus from Narita Airport to Downtown Tokyo. <br>
I turned on maps as usual and started to compare services.<br>
<br>
<br>
<br>
The two major map service providers depicted the real world in totally differenct way. <br>
<br>
Perhaps, Google is not really focusing on their maps on pedestrian perspectives.
<br>
<br>

Check out how the real world look like<br>
The pedestrian overpass goes under the expressway. 

<img src = "https://github.com/pil0706/pil0706.github.io/blob/master/screenshots/2nd/overpass_real.png?raw=true" width="400">

and these are how Apple and Google layered in their services

Apple | Google
-- |  --
![](https://github.com/pil0706/pil0706.github.io/blob/master/screenshots/2nd/overpass_apple.gif?raw=true) | ![](https://github.com/pil0706/pil0706.github.io/blob/master/screenshots/2nd/overpass_google.gif?raw=true) 

<br>
<br>
<br>
Data modelling wise, Apple is correct (or iPC, Apple Maps data provider in Japan). <br>
But, this is very bizarre that Apple's pedestrian overpass is disconnected.<br>
What it means is that the overpass goes under the expressway, they chose not to draw the hided parts.<br>
But, nice try but Apple created side-effects.<br>
It only works when the data goes with 'real-width road polygon'.<br>

> real-width road polygon : buffered polygon from road centerline with its real width

Google's pedestrian overpass seemed to look fine but it should go below the expressway.<br>
<br>
Both services did not illustrated the real world as it is.<br>
Or maybe both services are right according to their own policies or philsophy.
<br>
<br>
<br>
**Let's talk about side-effects of not using real-width road polygon.**
<br>
<br>
I love using **real-width road polygon** when the maps are zoomed-in.<br>
When it is used, the map becomes more abundant and spacious. <br>
'Spacious' is confusing term in map data, I guess, because it actually takes space on screen but spacious
<br>
<br>
Let's go back to the previous eyesoar.<br>
If Apple uses 'real-width road polygon', a center barrier of expressway could have been added without making disconnected pedestrian overpass.<br>
Yes using it can reduce bizzare looking and cartographers can add more features.
<br>
<br>
<br>
Check out an expressway in Japan. <br>
Google use 'real-width road polygon' so it showed toll booth and green areas on road (though now they changed their data).<br>
<br> 
On the other hand, Apple Maps does not show road facilities
<br>

![](https://github.com/pil0706/pil0706.github.io/blob/master/screenshots/2nd/tg_aVsg.gif?raw=true)


As far as I know, Japan and Korea are two countries provide the 'read-width road polygon' data.<br>
Nevertheless, Google applied real-width road polygon only in Japan.<br>
This is something I want to know why.
<br>
<br>
<br>
**Let's move on to downtown Tokyo. Who illustrated better? Modelling real-world.**
<br>
<br>
Tokyo, as one of the most complex cities in the world, is very hard to database-nized the city.
<br>
Countless overpass, pedestrian deck and overpass, bridges, _'a tunnel but highway ramp but also highway exit'_ are something you will never find in other countries.<br>
<br>
_Meguro Sky Garden_ is one of my landmark when I map Tokyo.
<br>
Oneday, I have noticed that something has changed on that landmark <br>
and a few days later it changed again.
<br>
![](https://github.com/pil0706/pil0706.github.io/blob/master/screenshots/2nd/meguro_google.gif?raw=true)

Yes, this was the day when Google has changed their data provider from Zenrin to their own.<br> 
Green areas and color of tunnel have added.<br>
So, Google is trying to depict the real world as accurate as possible.

> So, for those who are not familiar with Meguro Sky Garden,
> It is a building/condominium/but inside of it is expressway/ramp/exit/IC and on top of it is football field and garden.

Meguro Sky Garden is one big giant building at street level (and most of Tokyoite are walking or biking)<br>
From the aerial view, futsal field and skygarden are the two most outstanding features there.
![](https://github.com/pil0706/pil0706.github.io/blob/master/screenshots/2nd/meguro_now_streetlevel.png?raw=true)

> By the way, the cafe on the leftside is one of my favorite dessert/cafe in Nakameguro


The tunnel style improved a lot compared to the first version. <br>
But, I still do not see the building.
![](https://github.com/pil0706/pil0706.github.io/blob/master/screenshots/2nd/meguro_now.png?raw=true)
But, the new style doesn't seem to have features from pedestrian level nor aerial view.<br>


In fact, Apple's Meguro Sky Garden shows the 'greate circle' building (though there are not green areas)
![](https://github.com/pil0706/pil0706.github.io/blob/master/screenshots/2nd/apple_megro_building.png?raw=true)










Google announced Spatial Data Independence of Japan. <br>
I am sure their cartographers did know the side-effects of data independence <br>
Nevertheless, Google decided to do. <br>
Their decision process and drive are, I have to say, darn good.










- Appendix

Same Bug Vs. Not Good Endcap?

Google | Apple
-- | --
![](https://github.com/pil0706/pil0706.github.io/blob/master/screenshots/2nd/google_bug.gif?raw=true) | ![](https://github.com/pil0706/pil0706.github.io/blob/master/screenshots/2nd/apple_bug.gif?raw=true)







--- 한국어 버전
