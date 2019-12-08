---
layout: post
title: Learn from Apple & Google Maps | Apple & Google 지도로 부터 배우기
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
And from their mistakes, I have learned how to make/layer/design maps more precisely<br>
At least,  I'm trying not to make same mistakes they made.<br>
For certain areas, my map is better than theirs. <br>
<br>
<br>
<br>
Again, don't get me wrong. I love Apple products and devices with Google services<br>
<br>
<br>
<br>
I database-nized all these just because I have been making/designing/layering/analyzing maps for my work.
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

Check out how the real world looks like<br>
The pedestrian overpass goes under the expressway. 

<img src = "https://github.com/pil0706/pil0706.github.io/blob/master/screenshots/2nd/overpass_real.png?raw=true" width="400">

and these are how Apple and Google layered in their services

Apple | Google
-- |  --
![](https://github.com/pil0706/pil0706.github.io/blob/master/screenshots/2nd/overpass_apple.gif?raw=true) | ![](https://github.com/pil0706/pil0706.github.io/blob/master/screenshots/2nd/overpass_google.gif?raw=true) 

<br>
<br>
<br>
Data modeling wise, Apple is correct (or iPC, Apple Maps data provider in Japan). <br>
But, this is very bizarre that Apple's pedestrian overpass is disconnected.<br>
What it means is that the overpass goes under the expressway, they chose not to draw the hided parts.<br>
Nice try but Apple created side-effects.<br>
It only works when the data goes with 'real-width road polygon'.<br>

> real-width road polygon: buffered polygon from road centerline with its real width

Google's pedestrian overpass seemed to look fine but it should go below the expressway.<br>
<br>
Both services did not illustrate the real world as it is.<br>
Or maybe both services are right according to their own policies or philosophy.
<br>
<br>
<br>
**Let's talk about side-effects of not using real-width road polygon.**
<br>
<br>
I love using **real-width road polygon** when the maps are zoomed-in.<br>
When it is used, the map becomes more abundant and spacious. <br>
'Spacious' is a confusing term in map data, I guess because it actually takes space on-screen but spacious
<br>
<br>
Let's go back to the previous eyesore.<br>
If Apple uses 'real-width road polygon', a center barrier of expressway could have been added without making disconnected pedestrian overpass.<br>
Yes using it can reduce bizarre looking and cartographers can add more features.
<br>
<br>
<br>
Check out an expressway in Japan. <br>
Google uses 'real-width road polygon' so it shows toll booth and green areas on road (though now they changed their data).<br>
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
**Let's move on to downtown Tokyo. Who illustrated better? Modeling real-world.**
<br>
<br>
Tokyo, as one of the most complex cities in the world, is very hard to database-nized the city.
<br>
Countless overpass, pedestrian deck, and overpass, bridges, _'a tunnel but highway ramp but also highway exit'_ are something you will never find in other countries.<br>
<br>
_Meguro Sky Garden_ is one of my landmarks when I map Tokyo.
<br>
One day, I have noticed that something has changed on that landmark on Google Maps <br>
and a few days later it changed again.
<br>
![](https://github.com/pil0706/pil0706.github.io/blob/master/screenshots/2nd/meguro_google.gif?raw=true)

Yes, this was the day when Google has changed their data provider from Zenrin to their own.<br> 
Green areas and color of the tunnel have added.<br>
So, Google is trying to depict the real world as accurate as possible.

> So, for those who are not familiar with Meguro Sky Garden,
> It is a building/condominium/but inside of it is expressway/ramp/exit/IC and on top of it is a football field and garden.

Meguro Sky Garden is one big giant building at street level (and most of Tokyoite are walking or biking)<br>
From the aerial view, the futsal field and sky garden are the two most outstanding features there.
![](https://github.com/pil0706/pil0706.github.io/blob/master/screenshots/2nd/meguro_now_streetlevel.png?raw=true)

> By the way, the cafe on the left side is one of my favorite dessert/cafe in Nakameguro


The tunnel style improved a lot compared to the first version. <br>
Though I still do not see the building.
![](https://github.com/pil0706/pil0706.github.io/blob/master/screenshots/2nd/meguro_now.png?raw=true)
But, the new style doesn't seem to have features from pedestrian level nor aerial view.<br>


In fact, Apple's Meguro Sky Garden shows the 'greate circle' building (though there are not green areas)
![](https://github.com/pil0706/pil0706.github.io/blob/master/screenshots/2nd/apple_megro_building.png?raw=true)










Google announced the Spatial Data Independence of Japan. <br>
I am sure their cartographers did know the side-effects of data independence <br>
Nevertheless, Google decided to do it. <br>
Their decision process and drive are, I have to say, darn good.










- Appendix

Same Bug Vs. Not Good Endcap?

Google | Apple
-- | --
![](https://github.com/pil0706/pil0706.github.io/blob/master/screenshots/2nd/google_bug.gif?raw=true) | ![](https://github.com/pil0706/pil0706.github.io/blob/master/screenshots/2nd/apple_bug.gif?raw=true)







--- 한국어 버전


저의 예전 글로부터, <br>
다른 지도 서비스 제공자로부터 제가 찾은 에러들을 기록하고 있었습니다. <br>
대부분 Apple 과 Google 입니다.
<br>
<br>
<br>
이 글을 쓰기전에, <br>
저는 Apple과 Google의 직원들에게 뭐라고 하려고 하지 않습니다, 당신은 그들의 실수를 보게 될 것이지만요.
<br>
<br>
<br>
짧게 말하면, Apple은 아직 그들의 지도를 발전중에 있습니다. (Google 도..)
<br>
<br>
그리고, 그들의 실수로부터, 저는 지도를 더 정확하게 만들고/레이어링하고/디자인하는 법을 배웠습니다.<br>
적어도, 그들이 만든 같은 실수를 하지 않으려고 노력합니다.<br>
어떤 지역에서는, 제 지도는 그들의 것 보다 더 좋습니다.<br>
<br>
<br>
<br>
다시, 저를 잘못 이해하지 마세요. 저는 Apple의 제품과 Google의 서비스를 사랑합니다.<br>
<br>
<br>
<br>
저는 지도를 만들고/디자인하고/레이어링하고/분석하는 업무를 하기 때문에, 위 모든것들을 다 데이터베이스화 합니다.
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
**균형과 조화**
<br>
<br>
저는 이것들이 얼마나 중요한지 더이상 강조할 수 없습니다 (엄청 중요하다는 말)<br>
잘 훈련된 cartographers 라면 **균형과 조화**를 고려해야합니다.<br>
특별히, 지도 서비스에 있어서 그것들은 더 중요합니다, 지도 서비스는 모든 청중들을 만족시켜야 하니까요.
<br>
<br>
<br>
Apple 지도와 Google 지도는 균형이 잘 잡혀있습니다. (POIs 빼고요. POIs에 대해 할 말이 더 있습니다만, 이것들은 다음 글에 올릴 예정입니다.).<br>
하지만, 눈엣가시들이 존재합니다.<br>
그들의 데이터와 레이어 순서는 저를 약간 불편하게 만듭니다.
<br>
<br>
<br>
**육교에 대해서 이야기 해 봅시다.**
<br>
<br>
어느 날, 저는 나리타 공항에서 도쿄까지 오는 버스를 탔습니다.<br>
저는 평소와 같이 지도를 열었고, 각 서비스들을 비교하기 시작했습니다.<br>
<br>
<br>
<br>
그 두개의 지도 서비스는 이 세상을 다른 방식으로 묘사했습니다.<br>
<br>
아마도, Google은 보행자의 관점에 초점을 두지 않는 것 같습니다.
<br>
<br>

어떻게 실제 세상이 생겼는지 봅시다.<br>
육교는 고속도로 밑으로 지나 갑니다.

<img src = "https://github.com/pil0706/pil0706.github.io/blob/master/screenshots/2nd/overpass_real.png?raw=true" width="400">

그리고, 이것들은 어떻게 Apple과 Google의 서비스에서 레이어 되었는지 입니다.

Apple | Google
-- |  --
![](https://github.com/pil0706/pil0706.github.io/blob/master/screenshots/2nd/overpass_apple.gif?raw=true) | ![](https://github.com/pil0706/pil0706.github.io/blob/master/screenshots/2nd/overpass_google.gif?raw=true) 

<br>
<br>
<br>
데이터 모델링 측면에서, Apple이 맞습니다 (혹은 iPC, Apple 지도의 일본 데이터 제공자). <br>
하지만, Apple의 육교가 끊어져 있는것이 매우 이상합니다.<br>
무슨말이냐면, 육교가 고속도로 밑으로 지나가고, 그들은 숨겨진 지역을 그리지 않는것으로 선택했습니다.<br>
좋은 시도였지만, 애플은 부작용을 만들었습니다.<br>
이 방법은 데이터가 '실폭도로 폴리곤'과 함께 갈때 괜찮습니다.<br>

> 실폭도로 폴리곤 : 도로 중심선에서 실제 폭 만큼 버퍼된 것

Google의 육교는 괜찮아 보입니다, 하지만 이것은 고속도로 밑으로 지나가야 합니다.<br>
<br>
두개의 서비스는 실제와 달리 세상을 표현합니다.<br>
혹은 어쩌면 두개의 서비스는 그들의 자체의 정책이나 철학에 따라 맞습니다.
<br>
<br>
<br>
**실폭도로 폴리곤을 사용하지 않는것에 대해 부작용을 말해봅시다.**
<br>
<br>
저는 지도가 확대될 때 **실폭도로 폴리곤**을 사용하는것을 사랑합니다.<br>
그것들이 사용될때, 지도는 더 풍부해지고 더 넓어집니다.<br>
제 생각에, 지도 데이터에서 '넓어집니다'는 혼란스럽습니다, 왜냐하면 이것은 사실 스크린의 공간을 차지하지만 넓어지기 때문입니다.

<br>
<br>
방금의 눈엣가시로 돌아갑니다.<br>
만약 Apple이 '실폭도로 폴리곤'을 사용했다면, 고속도로의 중앙분리대가 육교의 끊어짐 없이 추가가 될 수 있습니다<br>
네 이것을 사용하면 이상한 모양을 줄일 수 있습니다 그리고 cartographers는 더 많은 요소들을 추가할 수 있습니다.
<br>
<br>
<br>
일본의 고속도로를 확인합니다. <br>
Google은 '실폭도로 폴리곤'을 사용합니다, 그래서 그것은 도로위 톨 부스라던지 녹지를 보여줍니다. (지금은 데이터를 교체했습니다.)<br>
<br> 
반면에, Apple 지도는 도로 시설을 보여주지 않습니다.
<br>

![](https://github.com/pil0706/pil0706.github.io/blob/master/screenshots/2nd/tg_aVsg.gif?raw=true)


제가 알기로, 한국과 일본은 '실폭도로 폴리곤' 데이터를 제공하는 두개의 나라입니다.<br>
그럼에도 불구하고, Google은 실폭도로 폴리곤을 일본에만 적용했습니다.<br>
이것은 왜 인지 제가 알고 싶은것 입니다.
<br>
<br>
<br>
**도쿄 시내로 움직입니다. 누가 더 잘 묘사했나? 실제 세상 모델링**
<br>
<br>
세상에서 가장 복잡한 도시중의 하나인 도쿄는 데이터화 하기 매우 어려운 도시입니다.
<br>
셀 수 없는 육교, 보행데크와 고가도로, 다리, _'터널이지만 고속도로 램프지만 고속도로 출구'_ 등은 다른 나라에서는 절대로 볼 수 없는 것입니다.<br>
<br>
_메구로 스카이 가든_ 은 내가 도쿄를 만들때 보는 랜드마크중 하나입니다.
<br>
어느날, 저는 그 랜드마크가 구글지도에서 변화된것을 확인했고 <br>
그리고 몇일 후 다시 변화된었습니다.
<br>
![](https://github.com/pil0706/pil0706.github.io/blob/master/screenshots/2nd/meguro_google.gif?raw=true)

네, 이날이 Google이 그들의 데이터를 Zenrin에서 자체 데이터로 바꾼 날 이었습니다.<br> 
녹지와 터널의 색상이 추가되엇습니다.<br>
그래서, Google은 세상을 정확하게 묘사하려고 노력합니다.

> 그래서, 메구로 스카이 가든을 잘 모르는 사람들에게,
> 이것은 건물/아파트/하지만 그 안에는 고속도로/램프/출구/IC 그리고 그 위에는 축구장과 정원이 있습니다.

메구로 스카이 가든은 거리에서는 하나의 큰 건물입니다 (그리고, 대부분의 도쿄시민들은 걷거나 자전거를 탑니다)<br>
공중에서 보면, 풋살장과 공중정원이 가장 눈에 띄는 요소입니다.
![](https://github.com/pil0706/pil0706.github.io/blob/master/screenshots/2nd/meguro_now_streetlevel.png?raw=true)

> 그나저나, 왼쪽의 카페는 제가 나카메구로에서 가장 좋아하는 디저트/카페입니다


터널의 스타일은 처음 버전보다 많이 개선 되었습니다. <br>
아직도 건물은 보이지 않습니다.
![](https://github.com/pil0706/pil0706.github.io/blob/master/screenshots/2nd/meguro_now.png?raw=true)
하지만, 새로운 스타일은 공중에서나 보행자 레벨에서의 요소들이 보이지 않습니다.<br>


사실, Apple의 메구로 스카이 가든은 '큰 원'건물을 보여줍니다 (그곳의 녹지는 없지만)

![](https://github.com/pil0706/pil0706.github.io/blob/master/screenshots/2nd/apple_megro_building.png?raw=true)










Google은 일본의 공간 데이터의 독립을 발표했습니다. <br>
저는 Google의 cartographers 가 데이터 독립의 부작용을 알았다고 확신합니다. <br>
그럼에도 불구하고, Google은 그렇게 결정했습니다. <br>
저는 그들의 결정 프로세스와 운행이 매우 좋다고 이야기 해야 합니다.










- 부록

같은 버그 Vs. 그냥 좋지 않은 Endcap?

Google | Apple
-- | --
![](https://github.com/pil0706/pil0706.github.io/blob/master/screenshots/2nd/google_bug.gif?raw=true) | ![](https://github.com/pil0706/pil0706.github.io/blob/master/screenshots/2nd/apple_bug.gif?raw=true)



