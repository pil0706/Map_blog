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
**Balance and harmony.** <br>
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
<br>
<br>
<br>
<br>
<br>
<br>
**Let's start with pedestrian overpass.**
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
<img src = "https://github.com/pil0706/pil0706.github.io/blob/master/screenshots/2nd/overpass_real.png?raw=true" width="400">

and these are how Apple and Google layered in their services

Apple | Google
-- |  --
![](https://github.com/pil0706/pil0706.github.io/blob/master/screenshots/2nd/overpass_apple.gif?raw=true) | ![](https://github.com/pil0706/pil0706.github.io/blob/master/screenshots/2nd/overpass_google.gif?raw=true) 



Data modelling wise, Apple is correct (or iPC, Apple Maps data provider in Japan). Because the pedestrian overpass is under the expressway.<br>
But, this is very eyesoar to me that Apple did not choose to use 'real-width road polygon', weird detachement or disconnection of disconnection of the pedestrian overpass is occured, once zoomed-in. <br>

(real-width road polygon : buffered polygon from road centerline with its real width)

Google seemed to okay but it should go below the expressway.<br>
Both are wrong, or maybe both are right according to their own mapping policy or mapping philsophy.




- Let's talk about side effects of not using real-width road polygon.

I love using real-width road polygon when the maps are zoomed-in.<br>
When it is used, the map becomes more abundant and spacious. <br>
'Spacious' could cause mis-understanding, because it actually takes space on screen but spacious? <br>
Yes, it takes space but other facilites can be on top of it, such as pedestrian crossing, bridge columns, and other pedestrian/human friendly facilities.



Check out the expressway in Japan. <br>
Google uses (at this time, they used Zenrin data) real-width road polygon so it showed toll booth and green areas on road.<br>
On the other hand, Apple Maps is simple. (yes I know simple is the best)<br>

![](https://github.com/pil0706/pil0706.github.io/blob/master/screenshots/2nd/tg_aVsg.gif?raw=true)


As far as I know, Japan and Korea are two countries provide the data.<br>
Nonetheless, Google applied real-width road polygon only in Japan. This is something I want to know why.








- Let's move on to downtown Tokyo. Who illustrated better? Modelling real-world.


Tokyo, as one of the most complex cities in the world, is very hard to spatialize the city. <br>
Countless overpass, pedestrian deck and overpass, bridges, 'a tunnel but highway ramp but also highway exit' are something you will never find in other countries.<br>

Meguro Sky Garden is one of my landmark when I map Tokyo.

Oneday, I have noticed that something has changed on that landmark <br>
and a few days later it changed again.
![](https://github.com/pil0706/pil0706.github.io/blob/master/screenshots/2nd/meguro_google.gif?raw=true)

Yes, this was the day when Google has changed their data provider from Zenrin (Zenrin Web) to their own.<br> 
You see the style is being changed and trying to illustrate the real world as accurate as possible?





> So, for those who are not familiar with Meguro Sky Garden,
> It is a building/condominium/but inside of it is expressway/ramp/exit/IC and on top of it is football field and garden.



The tunnel style improved a lot compared to the first version. <br>
But, it does not look like a tunnel still I do not see the building. (I should expose myself more to Google to get used to their new style in Japan).
![](https://github.com/pil0706/pil0706.github.io/blob/master/screenshots/2nd/meguro_now.png?raw=true)


Meguro Sky Garden is one big giant building at street level (and most of Tokyoite are walking or biking)<br>
From the aerial view, futsal field and skygarden are the two most outstanding features there.
![](https://github.com/pil0706/pil0706.github.io/blob/master/screenshots/2nd/meguro_now_streetlevel.png?raw=true)


But, the new style doesn't seem to have them.<br>
> By the way, the cafe on the leftside is one of my favorite dessert/cafe in Nakameguro

In fact, Apple's Meguro Sky Garden shows the 'greate circle' building
![](https://github.com/pil0706/pil0706.github.io/blob/master/screenshots/2nd/apple_megro_building.png?raw=true)










Google announced Spatial Data Independence of Japan. <br>
I am sure their cartographers did know the side-effects of data independence <br>
Nevertheless, Google decided to do. Their decision process and drive are, I have to say, darn good.










- Appendix

Same Bug Vs. Not Good Endcap?

Google | Apple
-- | --
![](https://github.com/pil0706/pil0706.github.io/blob/master/screenshots/2nd/google_bug.gif?raw=true) | ![](https://github.com/pil0706/pil0706.github.io/blob/master/screenshots/2nd/apple_bug.gif?raw=true)







--- 한국어 버전
