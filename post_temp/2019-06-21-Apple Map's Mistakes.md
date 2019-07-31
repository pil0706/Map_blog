---
layout: post
title: Learn from others - Apple and Google (2/2) / 다른사람의 실수로부터 배우기 - Apple 과 Google (2/2)
---

From the previous story, </br>
I am going to continue to write errors which I have found from other map service providers. </br>
Most likely Apple and Google.

Before I start to write article, I have to make it clear that I am not attacking employees in Apple and Google though you are going to see their mistakes.



Long story short, Apple still needs to improve their maps. (or maybe I am biased?)</br>
I have learned a lot from others ~~(from their mistakes)~~ and I am trying not to make same mistakes they made. </br>
For certain areas, my map is better than theirs. </br>


Again, don't get me wrong. I love Apple products and devices (Watch, AirPod, iPhone, iMac, Macbook <- yes, these are what I use everyday) </br>
I love Google services.


All these is based on my instinct/feeling/thoughts of their maps after analyzing their maps for 2 years.








Balance and harmony. </br>
I can't emphasize enough on the importance of them. </br>
Well trained cartographers should check balance and harmony when they make maps. If their maps also contain the real world features as it is, no one is going to say bad thigns about it.



I believe Apple and Google is very well balanced (except POIs. I have more things to say POIs but it will come to next article).</br>
Most of things that makes me uncomfortable is the data (or bugs) or layering orders.





- Let's start with pedestrian overpass.

One day, I took a bus from Narita Airport to Downtown Tokyo. </br>
I turned on maps and started to compare services. (It's my habit. I do everyday.) </br>

The two major map service providers depicted the real world in totally differenct way. </br>
Perhaps, Google is not really focusing on their maps on pedestrian perspectives.


Google | Apple | Real World
-- | -- | --
![](https://github.com/pil0706/pil0706.github.io/blob/master/screenshots/2nd/overpass_google.gif) | ![](https://github.com/pil0706/pil0706.github.io/blob/master/screenshots/2nd/overpass_apple.gif) | ![](https://github.com/pil0706/pil0706.github.io/blob/master/screenshots/2nd/overpass_real.png)





Data modelling wise, Apple is correct (or iPC, Apple Maps data provider in Japan). Because the pedestrian overpass is under the expressway.</br>
But, this is very eyesoar to me that Apple did not choose to use 'real-width road polygon', weird detachement or disconnection of disconnection of the pedestrian overpass is occured, once zoomed-in. </br>

(real-width road polygon : buffered polygon from road centerline with its real width)

Google seemed to okay but it should go below the expressway.</br>
Both are wrong, or maybe both are right according to their own mapping policy or mapping philsophy.




- Let's talk about side effects of not using real-width road polygon.

I love using real-width road polygon when the maps are zoomed-in.</br>
When it is used, the map becomes more abundant and spacious. </br>
'Spacious' could cause mis-understanding, because it actually takes space on screen but spacious? </br>
Yes, it takes space but other facilites can be on top of it, such as pedestrian crossing, bridge columns, and other pedestrian/human friendly facilities.



Check out the expressway in Japan. </br>
Google uses (at this time, they used Zenrin data) real-width road polygon so it showed toll booth and green areas on road.</br>
On the other hand, Apple Maps is simple. (yes I know simple is the best)</br>

![](https://github.com/pil0706/pil0706.github.io/blob/master/screenshots/2nd/tg_aVsg.gif)


As far as I know, Japan and Korea are two countries provide the data.</br>
Nonetheless, Google applied real-width road polygon only in Japan. This is something I want to know why.








- Let's move on to downtown Tokyo. Who illustrated better? Modelling real-world.


Tokyo, as one of the most complex cities in the world, is very hard to spatialize the city. </br>
Countless overpass, pedestrian deck and overpass, bridges, 'a tunnel but highway ramp but also highway exit' are something you will never find in other countries.</br>

Meguro Sky Garden is one of my landmark when I map Tokyo.

Oneday, I have noticed that something has changed on that landmark </br>
and a few days later it changed again.
![](https://github.com/pil0706/pil0706.github.io/blob/master/screenshots/2nd/meguro_google.gif)

Yes, this was the day when Google has changed their data provider from Zenrin (Zenrin Web) to their own.<br> 
You see the style is being changed and trying to illustrate the real world as accurate as possible?





> So, for those who are not familiar with Meguro Sky Garden,
> It is a building/condominium/but inside of it is expressway/ramp/exit/IC and on top of it is football field and garden.


The tunnel style improved a lot compared to the first version. </br>
But, it does not look like a tunnel still I do not see the building. (I should expose myself more to Google to get used to their new style in Japan).
![](https://github.com/pil0706/pil0706.github.io/blob/master/screenshots/2nd/meguro_now.png)


Meguro Sky Garden is one big giant building at street level (and most of Tokyoite are walking or biking)</br>
From the aerial view, futsal field and skygarden are the two most outstanding features there.
![](https://github.com/pil0706/pil0706.github.io/blob/master/screenshots/2nd/meguro_now_streetlevel.png)
But, the new style doesn't seem to have them.</br>
(By the way, the cafe on the leftside is one of my favorite dessert/cafe in Nakameguro)


So, I have to raise a hand for Zenrin
So, what I can tell you is that I see Google is being improved. But I do not know Apple.







Google announced Spatial Data Independence of Japan. </br>
I am sure their cartographers did know the side-effects of data independence </br>
Nevertheless, Google decided to do. Their decision process and drive are, I have to say, darn good.










- Appendix

Same Bug Vs. Not Good Endcap?
Google | Apple
-- | --
![](https://github.com/pil0706/pil0706.github.io/blob/master/screenshots/2nd/google_bug.gif) | ![](https://github.com/pil0706/pil0706.github.io/blob/master/screenshots/2nd/apple_bug.gif)







--- 한국어 버전