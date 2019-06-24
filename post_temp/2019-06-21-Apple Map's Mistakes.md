---
layout: post
title: Japan, Probably the most difficult country to Service Providers' Mistakes / 지도 서비스 회사의 실수
---

I am going to start with a screenshot of Apple and Google Maps

![AppleVsGoogle](https://github.com/pil0706/pil0706.github.io/blob/master/screenshots/2nd/aVsg_edit.png)

To not to get distracted from POI and Labels, I got rid of them all.

These type of residence is usually in the southeast Asia. But, the maps are somewhere in Japan
![](https://i.pinimg.com/originals/3a/9b/cd/3a9bcd20ab39bf79bfab51c2ad033bca.jpg)

In fact, I have reported last year through Twitter and Apple asked me where that is ~~(I am not going to tell them until they offer me a position overthere)~~.
![TwitterScreenshot](https://github.com/pil0706/pil0706.github.io/blob/master/screenshots/2nd/twitter_screenshot.png)



Anyway, I, often, see their mistakes. What I do is take a snapshot of them (I am happy when I find them out for no reasons) and I always think that I should not make that mistake when I make my map.




Again, Japan, a country I like, 
Not just because I have nothing to do, I do wonder around Japan through Apple Maps and Google Maps very often.



Buildings on water in Japan, that's very おかしい（weird).
I was just curious why they did make same mistakes, because my map does not have that bizarre phenomenon.
![](https://github.com/pil0706/pil0706.github.io/blob/master/screenshots/2nd/myMap.png)

I came out with conclusions below, which causes this phenomenon.
1. Data did not come from one source
    - for instance, water bodies, buildings, road links all are from difference sources
2. Like the Bermuda triangle, only that part of world has projection bugs
	- when service providers convert spatial data to vector tiles, that area has 'unknown' issues? (I maybe go too far. I don't want to believe they made that mistakes.)
3. I may be wrong

So, I tracked their data down as much as I could.

Google's data provider's attribution can be easily found and it used to be Zenrin but now it does not show anything.
![](https://github.com/pil0706/pil0706.github.io/blob/master/screenshots/2nd/google_attribution.png)
In other countries, you still can find the data providers but not in lower level (or in small scale)
![](https://github.com/pil0706/pil0706.github.io/blob/master/screenshots/2nd/google_attribution_changes.gif)


Apple announced that they use Increment P Corp. data for Japan and I assumed that possible open-sourced data providers are WAZE, OSM.


But, Google probably did not make water bodies or their data from scratch.
Let me track them down.

OSM and Natural Earth are probably the easiest open-sourced spatial data provider so I started to check their data first.
 - Natural Earth
 - Open Street Map (planet.osm.pbf)
 - Openstreetmap Data (https://osmdata.openstreetmap.de)

Natural Earth provides as accurate as 1 to 10 Million scale, I guess I do not have to download them but I did.
![](https://github.com/pil0706/pil0706.github.io/blob/master/screenshots/2nd/tokyo_bay.png)
Okay, it is too obvious.

Let's go with Open Street Map's water area.
This is a little bit tricky though I had to install osmosis to extract water bodies and OGR convert them to familiar format like 'shape'. OSM Taginfo is really pain in the butt but I just used natural=water and natural=coastline.
for more detail, you may go here https://taginfo.openstreetmap.org/keys/natural#values
(you could use imposm3 and postgis but this isn't my work related so I use the simplest way to do)

I downloaded world osm.pbf file and extracted water boundaries only.
You can try with the planet site but it will take forever to download (for 24 hours, with my house network (the cheapest and lowest network speed) and my iMac (i5 3.2GHz, 24GB 1600 MHz) was only able to download 16% of planet data). I used geofabrik instead, where you can specify your target country/region.




After I did extract and convert the data, I could just show you openstreetmap because it is basically same as the planet.osm.pbf and I just noticed that QGIS reads .osm.pbf (There always are easiest and fastest way to achieve your goal.)


This is the result of OSM Buildings in that bizarre area.
- No OSM Building provided in OSM.PBF
- Google and Apple seemed to have the river in polygon but OSM provides only line





OpenMaptiles' Water Boundary's diagram is illustrated below
https://github.com/openmaptiles/openmaptiles/raw/master/layers/water/etl_diagram.png?raw=true





This was my guess that the water polygons (ocean layer) or land polygons is not compatible with buildings in Japan



http://www.geonames.org



Apple has started their map servie in year 2012

All their products are iOS or Mac OS based applications so optimization probably 
They do not have service on Web

Justine Obeirne 


Apple Maps Mistakes (POI/ICON/Buildings on Water/음차/)

-Apple Maps Water Bodies?
 - Natural Earth
 - OSM
 - OpenMapTiles (https://github.com/openmaptiles)
 - Openstreetmap Data (https://osmdata.openstreetmap.de)


OpenMaptiles' Water Boundary's diagram is illustrated below
https://github.com/openmaptiles/openmaptiles/raw/master/layers/water/etl_diagram.png?raw=true


osm water bodies using osmosis and osm taginfo (https://taginfo.openstreetmap.org)

natural earth from web.. Too simplified



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






--- 한국어 버전