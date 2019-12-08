---
layout: post
title: Learn from Others Mistakes | 다른사람의 실수로부터 배우기
---

I am going to start with screenshots of Apple (L) and Google (R) Maps without labels and POIs.

<p align="center">
 <img src="https://github.com/pil0706/pil0706.github.io/blob/master/screenshots/2nd/aVsg_edit.png?raw=true">
</p>


I have found out a few buildings on water bodies, as you may notice from the screenshots. <br>
This type of residence is usually in the Southeast Asia.<br>
But, you are looking at somewhere in Japan.

<p align="center">
 <img widht="600" height="600" src="https://i.pinimg.com/originals/3a/9b/cd/3a9bcd20ab39bf79bfab51c2ad033bca.jpg">
</p>


In fact, I reported last year through Twitter and Apple asked me where that was.<br>
And I lost their contacts.<br>

<p align="center">
 <img widht="300" height="300" src="https://github.com/pil0706/pil0706.github.io/blob/master/screenshots/2nd/twitter_screenshot.png?raw=true">
</p>

Japan as a country I like,<br>
I do wonder around Japan through Apple and Google Maps quite often<br> and try to capture as many mistakes as I can.<br>
<br>
<br>
Those databases help me not to make same mistakes (on that location) as they have made and it really does help my map look better.
<br>
<br>
Anyway,<br>
buildings on water, that's very おかしい (weird).<br>
I was just curious why they did make the same mistakes because my map looks just fine. (the screenshot below is my map in the same spot)
<p align="center">
 <img widht="600" height="600" src="https://github.com/pil0706/pil0706.github.io/blob/master/screenshots/2nd/myMap.png?raw=true">
</p>

I came out with conclusions below, which causes this phenomenon: buildings on water.<br>

**Data did not come from one source**<br>

> for instance, water bodies, buildings, road links all are from different sources

**Like the Bermuda triangle, only that part of the world has projection bugs**<br>

> when service providers convert spatial data to vector tiles, that area has 'unknown' issues? (I maybe went too far. I don't want to believe they made those mistakes.)

**I may be wrong**<br>


So, I tracked their **data sources** first.<br>

<br>
<br>
Google's data provider's attribution can be easily found and it used to be Zenrin but now it does not show anything.
<p align="center">
 <img widht="600" height="600" src="https://github.com/pil0706/pil0706.github.io/blob/master/screenshots/2nd/google_attribution.png?raw=true">
</p>
In other countries (Singapore, in the follwing screenshots), you still can find the data providers but not in lower zoom level.

<p align="center">
 <img src="https://github.com/pil0706/pil0706.github.io/blob/master/screenshots/2nd/google_attribution_changes.gif?raw=true">
</p>


Apple announced that they use Increment P Corp. data for Japan. <br>
<br>
<br>

But, Increment P or Zenrin provide the global water bodies?<br>
<br>
<br>

I believe Apple and Google probably drew global water bodies from 'somewhere' and made details after.<br>
Which means that they did not make water bodies from the scratch.<br>
<br>
<br>

I assumed that possible open-source data could be added to Apple and Google Maps are WAZE, OSM, and Natural Earth.

<br>
<br>
So, I tracked possible open-source data down one by one.
<br>
- 1. Natural Earth<br>
- 2. Open Street Map (planet.osm.pbf)<br>
- 3. Openstreetmap Data -> [Data Web](https://osmdata.openstreetmap.de)

<br>

1. **Natural Earth**<br>
they provide as accurate as 1 to 10 Million scale, I guess I do not have to download them but I did.

<p align="center">
 <img widht="600" height="600" src="https://github.com/pil0706/pil0706.github.io/blob/master/screenshots/2nd/tokyo_bay.png?raw=true">
</p>
Okay, it is too obvious.

2. **Open Street Map**<br>
Let's go with Open Street Map's water area.

This is a little bit tricky though <br>
I had to install osmosis to extract water bodies and OGR convert them to familiar format like 'shape'.<br>
<br>
<br>
OSM Taginfo is really pain in the butt<br>
but I just used natural=water and natural=coastline.<br>
<br>
<br>
for more detail, you may go here -> [OSM taginfo](https://taginfo.openstreetmap.org/keys/natural#values)

> (you could use imposm3 and PostGIS but this isn't my work-related so I use the. simplest way to do)


I downloaded world osm.pbf file and extracted water boundaries only.

> You can try with the planet site but it will take forever to download (for 24 hours, with my house network and my iMac (i5 3.2GHz, 24GB 1600 MHz) was only able to download 16% of planet data).

I used geofabrik instead, where you can specify your target country/region.

After I did extract and convert the data, I could just show openstreetmap because it is the same as planet.osm.pbf (There always are the easiest and fastest way to achieve your goal.)



These are the data results of the bizarre area.<br>
- No OSM Building provided in OSM.PBF
- Google and Apple seemed to have the river in polygon but OSM provides the only line

Here's the data I extracted from OSM.PBF and Openstreetmap

<p align="center">
 <img src="https://github.com/pil0706/pil0706.github.io/blob/master/screenshots/2nd/osm.gif?raw=true">
</p>


3. **Openstreetmap Data : [Data Download Link](https://osmdata.openstreetmap.de)**<br>
I guess I don't have much expectation on their data..

<p align="center">
 <img src="https://github.com/pil0706/pil0706.github.io/blob/master/screenshots/2nd/opendata.png?raw=true">
</p>
 
The coastline detail is much better than OpenStreetMap or Natural Earth though inland waterbodies didn't exist.
<br>
<br>
So... what now, what's left?
<br>
<br>
**Projection?**<br>
<br>
But, would it be possible that both services have the same projection bugs in the same area?
<br>
<br>
**I am wrong?**<br>
<br>
I was not able to get building polygons from both Google and Apple. <br>
<br>
But what I can tell is the water polygons or land polygons are not compatible with buildings in Japan.<br>
This applies to both services coincidentally.
<br>
<br>
Other trivial errors, it was meaningless to post them here.<br>
But buildings on water phenomena were somewhat eyesore to me and I decided to post.



--- 한국어 버전

Label과 POI를 제거한 Apple (왼)과 Google (오)지도의 스크린샷으로 시작하겠습니다.

<p align="center">
 <img src="https://github.com/pil0706/pil0706.github.io/blob/master/screenshots/2nd/aVsg_edit.png?raw=true">
</p>

스크린샷에서 보시다시피, 몇개의 건물들이 물위에 있는것을 발견하였습니다.<br>
이러한 건물 타입은 주로 동남아시아에서 볼 수 있는 것 입니다.<br>
하지만, 여러분들은 일본의 어느 지역을 보고 계십니다.

<p align="center">
 <img widht="300" height="300" src="https://i.pinimg.com/originals/3a/9b/cd/3a9bcd20ab39bf79bfab51c2ad033bca.jpg?raw=true">
</p>


사실, 작년에 트위터를 통해 공개했고, 애플이 반응을 보였습니다. 그리고 전 그들의 연락을 잃었죠.
<p align="center">
 <img widht="600" height="600" src="https://github.com/pil0706/pil0706.github.io/blob/master/screenshots/2nd/twitter_screenshot.png?raw=true">
</p>




일본은 제가 좋아하는 나라로써,<br>
Apple과 Google 지도로 자주 돌아다닙니다 그리고 얘네들이 만든 실수를 캡쳐하려고 노력합니다.<br>
이렇게 축척된 데이터베이스는 같은 실수를 반복하지 않게 도와주고, 실제로 이걸 통해서 제 지도는 Apple과 Google이 만든 실수를 안하도록 도와주고 결과도 더 좋습니다.


어쨋던,<br>
물위에 있는 건물은 매우  おかしいです (이상합니다).<br>
저는 그냥 궁금했습니다, 제 지도는 괜찮은데 왜 얘네들이 같은 실수를 만들었는지.
<p align="center">
 <img widht="600" height="600" src="https://github.com/pil0706/pil0706.github.io/blob/master/screenshots/2nd/myMap.png?raw=true">
</p>

이와 같은 현상에 저는 아래와 같은 결론을 내렸습니다.<br>

**A**. 데이터의 출처가 여러곳이다<br>

> 예를들면, 수계, 건물, 도로 등 다 여기저기서 온것입니다.

**B**. 버뮤다 삼각지대 같이, 이 지역에서만 생기는 투영법 버그<br>

> 벡터 타일로 서비스를 할때 유독 이 지역에서만 생기는 '알수없는' 이슈? (아마도 제가 너무 많이 간 것 같습니다. 얘네들이 이런 실수를 했을거라고 믿고 싶지 않습니다.)

**C**. 내가 틀림<br>


그래서, 얘네들의 데이터를 추적하기로 했습니다.<br>
구글의 데이터 제공업체는 쉽게 찾을 수 있습니다. 과거에는 젠린이었지만, 지금은 아무것도 없네요
<p align="center">
 <img widht="600" height="600" src="https://github.com/pil0706/pil0706.github.io/blob/master/screenshots/2nd/google_attribution.png?raw=true">
</p>
다른 나라에서는, 데이터 제공업체를 찾을 수 있습니다, 하지만 낮은 레벨에서는 아니네요.
<p align="center">
 <img src="https://github.com/pil0706/pil0706.github.io/blob/master/screenshots/2nd/google_attribution_changes.gif?raw=true">
</p>



Apple은 Increment P Corp.의 데이터를 사용한다고 알렸습니다. 그리고 추측할 수 있는 다른 데이터는 WAZE, OSM 정도일 겁니다.



Google은 아마도 처음부터 수계와 다른 데이터를 만들지 않았을 거라고 생각했습니다.<br>
그래서 추적을 합니다.

OSM 과 Natural Earth는 아마 가장 쉬운 공개된 데이터이지 않을까 합니다. 그래서 얘네들의 데이터를 먼저 확인해보았습니다.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 1. Natural Earth<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 2. Open Street Map (planet.osm.pbf)<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 3. Openstreetmap Data -> [Data Web](https://osmdata.openstreetmap.de)

A.1. **Natural Earth**<br>
얘네가 제공하는 데이터의 정확도는 1 : 1000만, 다운받을 가치도 없겟지만 해봅니다.
<p align="center">
 <img widht="600" height="600" src="https://github.com/pil0706/pil0706.github.io/blob/master/screenshots/2nd/tokyo_bay.png?raw=true">
</p>
네, 너무 명확합니다.

A.2. **Open Street Map**<br>
Open Street Map의 수계를 열어봅니다.

이거는 약간 꼼수인데, osmosis와 OGR을 이용하여 수계를 추출합니다. <br>
OSM Taginfo 는 정말로 짜증나지만 다음과 같은 필터 조건을 사용했습니다 natural=water and natural=coastline.<br>
더 자세한 정보는 여기로 가십시요 -> [OSM taginfo](https://taginfo.openstreetmap.org/keys/natural#values)

> (imposm3와 postgis를 사용할 수 있지만, 제 업무와 관련된 일이 아니기에 그냥 쉬운 방법으로 갑니다)

세계 osm.pbf 파일을 다운받고 수계만 추출했습니다.

> 다운받는데 오래 걸렸습니다. (24시간 동안, 저의 집의 네트워크와 제 iMac (i5 3.2GHz, 24GB 1600 MHz)으로 16% 밖에 못받고 있더군요).그래서 geofabrik 을 대신 사용했습니다. 원하는 국가/지역을 선택할 수 있습니다. 추출하고, 데이터를 변환했습니다.<br>
> 그냥 openstreetmap을 보여줘도 될 거라는 생각을 했습니다. 왜냐하면 기본적으로 같기 때문입니다. (항상 목표로 도달하기 위한 쉽고 빠른길이 있더군요)

이상한 지역에 대한 데이터 결과 입니다.<br>
- 빌딩 없음
- Google 과 Apple 의 강은 polygon 이나 OSM 은 line

여기, OSM에서 추출한 데이터와 Openstreetmap을 보여드립니다.
<p align="center">
 <img src="https://github.com/pil0706/pil0706.github.io/blob/master/screenshots/2nd/osm.gif?raw=true">
</p>


A.3. **Openstreetmap Data -> [Data Web](https://osmdata.openstreetmap.de)**<br>
이 데이터에 대한 기대가 없습니다..
<p align="center">
 <img src="https://github.com/pil0706/pil0706.github.io/blob/master/screenshots/2nd/opendata.png?raw=true">
</p>
해안선은 OpenStreetMap or Natural Earth보다 디테일하지만 내륙에 수계는 없습니다.


그럼, 이제 뭐지? 뭐가 남았지?


B. 투영법?<br>
하지만, 두개의 서비스 회사가 같은 지역에 같은 문제가 있을거라 생각하지 않습니다.

C. 내가 틀렸나?<br>
그냥 모르겠습니다.<br>
Google 과 Apple의 건물을 구할 수 없었습니다.<br>
하지만, 하나 말할 수 있는것은 일본에서 수계 혹은 땅과 건물이 일치하지 않는 것 입니다. 공교롭게도 두개의 서비스 회사에서 같이 적용됩니다.



다른 사소한 실수들은 여기에 올리는것이 의미가 없었습니다.<br>
하지만, 이 현상은 저에게 눈엣가시였기에 올리는 계기가 되었습니다.