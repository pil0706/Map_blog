---
layout: post
title: Learn from others mistakes (2/2) / 다른사람의 실수로부터 배우기 (2/2)
---

From the previous story, I am going to continue what I have found from other map service providers.




여기부터 내용 수정좀 하자



Apple has started their map servie in year 2012

All their products are iOS or Mac OS based applications so optimization probably 
They do not have service on Web

Justine Obeirne 


Apple Maps Mistakes (POI/ICON/Buildings on Water/음차/)





육교
One day, I took a bus from Narita Airport to Downtown Tokyo. All of sudden, I turned on the map and 
Google : ![](https://github.com/pil0706/pil0706.github.io/blob/master/screenshots/2nd/overpass_google.gif)
Apple : ![](https://github.com/pil0706/pil0706.github.io/blob/master/screenshots/2nd/overpass_apple.gif)

Real World : ![](https://github.com/pil0706/pil0706.github.io/blob/master/screenshots/2nd/overpass_real.png)

Data modellign wise, Apple is correct (or iPC) but because they did not choose to use real-width road shape, weird disconnection of the pedestrian overpass is eyesoar
Google seemed to okay but it should go below the express highway
Both are wrong, or maybe both are right according to their own mapping policy or philsophy.




실폭도로
![](https://github.com/pil0706/pil0706.github.io/blob/master/screenshots/2nd/tg_aVsg.gif)




So, this is my conclusion that Apple is combining all the data from here and there and 
(But, maybe I am wrong)


Tokyo, as one of the most complex cities in the world, is very hard to spatialize the city. Countless overpass, pedestrian deck, bridges, tunnel but highway ramp but also highway exit are something you will never find in other countries.
Meguro Sky Garden is one of my landmark when I map Tokyo.

Google has changed their data provider from Zenrin (Zenrin Web) to their own. And Google Maps (Japan) is improving day by day.
![](https://github.com/pil0706/pil0706.github.io/blob/master/screenshots/2nd/meguro_google.gif)


It improved much and it does not look like a tunnel still I do not see the building
![](https://github.com/pil0706/pil0706.github.io/blob/master/screenshots/2nd/meguro_now.png)
Because Meguro Sky Garden is one big giant building on street level (and most of Tokyoite are waking or biking)
From the aerial view, futsal field and skygarden are the two most outstanding features there.
![](https://github.com/pil0706/pil0706.github.io/blob/master/screenshots/2nd/meguro_now_streetlevel.png)
(By the way, the cafe on the leftside is one of my favorite dessert/cafe in Nakameguro)
So, I have to raise a hand for Zenrin


But, Google announced Spatial Data Independence of Japan. I have to say they are darn badass.










Same Bug Vs. Not Good Endcap?
Google Vs. Apple

Google | Apple
-- | --
![](https://github.com/pil0706/pil0706.github.io/blob/master/screenshots/2nd/google_bug.gif) | ![](https://github.com/pil0706/pil0706.github.io/blob/master/screenshots/2nd/apple_bug.gif)












Trivial errors, it was meaningless to post them here. But these phenomena were very dramatic and I decided to post and share my thoughts on this.




--- 한국어 버전