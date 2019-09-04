---
layout: post
title: Hopping Labels : Map Label Placement - Copenhagen Pikabu | 뛰어 다니는 레이블(주기) : 지도 레이블(주기) 위치 - 코펜하겐 까꿍
---

### Label, the Finale of Cartography

Because of limited space, <br>
it is always hard to show all the labels on a map.
<br>
<br>
Let's say you are in a situation of labeling names of countries, especially in a lower zoom level.
<br>
<br>
Each one of labels are very important.<br>
If a country's label is hided or overlapped by another country's, someone might be upset.
<br>
<br>
Therefore, cartographers must choose what to show or where to locate labels under a clear policy.
<br>
<br>
One day,<br>
one of my colleagues asked me, can a label of Portugal be shown in low zoom level.
<br>
<br>
For instance, adjacent countries, Spain and Portugal,<br>
Portugal might not show up, for Spain takes space.<br>
In other words, there is no enough space to pose the label of Portugal.
<br>
<br>
<img src="https://github.com/pil0706/pil0706.github.io/blob/master/screenshots/positionofpois/no_portu.png?raw=true">
<br>
<br>
If I were a Portuguese, I might be upset.
<br>
However, if the cartographer is Spanish?<br>
Spain comes first than Portugal, for his sake.
<br>
<br>
To not to get egged, I see that Google Maps adjusts the labels in each zoom level.
<br>
<br>
<img src="https://github.com/pil0706/pil0706.github.io/blob/master/screenshots/positionofpois/portu_location_change.gif?raw=true">
<br>
<br>
From Zoom Lv5, it seems like the label keeps its position till it gets dissapeared.
<br>
On the other hand, Apple Maps does seem to change labels location.
<br>
<br>
<img src="https://github.com/pil0706/pil0706.github.io/blob/master/screenshots/positionofpois/portu_location_change_apple.gif?raw=true">
<br>
<br>
Apple Maps keeps their lable position consistently; on the other hand, Google Maps is more flexible in their label position.
<br>
<br>
Based on my almost 9 years of map making experiences, it's obvious that Apple Maps and Google Maps adjust the place labels manually.

> the place lables can be defined as labels of countries, cities, airport, etc.

I can tell they are not using centroid of each countries.
<br>
I used 'Centroid on Surface' to have center points of each countries.<br>
<br>
Here, I drew lines between centroid points of each contries from Natural Earth data and Google Maps place labels.
<br>
<br>

<img src="https://github.com/pil0706/pil0706.github.io/blob/master/screenshots/positionofpois/naturalearth_google.gif?raw=true">

<br>
<br>
The reason why I am showing this is that<br>
I want to emphasize Google Maps and Apple Maps did not just use simple centroid for labeling<br>
<br>
Instead, **someone** (and I strongly believe that he or she is a very well cartographer who carries Google and Apple's internal policies or philosophies) manually replotted them.
<br>
<br>

<img src="https://github.com/pil0706/pil0706.github.io/blob/master/screenshots/positionofpois/ne_google_z4.png?raw=true">
<br>
<br>

Also, Google Maps changes their location level by level.<br>
On the other hand, Apple sets its initial location and uses all zoom levels
<br>
<br>

<img src="https://github.com/pil0706/pil0706.github.io/blob/master/screenshots/positionofpois/apple_google_z4.png?raw=true">

> I tried to match Apple's Zoom level to Google's Zoom Level but this was the best I could do.

<img src="https://github.com/pil0706/pil0706.github.io/blob/master/screenshots/positionofpois/apple_google_overlap.png?raw=true">
<br>

> and finally ended up matching Apple Maps and Google Maps with same scale


<br>
<br>
I marked the center point of country labels in ZLv3 and Zlv4 in Apple Maps.<br>
Further, I re-sized (reduced) Zlv4 to match to Zlv3, in order to compare position of Apple Maps' country label positions.

<img src="https://github.com/pil0706/pil0706.github.io/blob/master/screenshots/positionofpois/apple_eu_z3z4_overlap_again.png?raw=true">

<br>
<br>
With my shaking hands and PowerPoint's auto snapping, the lables position remained almost in same spots in every labels in Apple Maps.

Z3-Z4 | Z4-Z5
-- | --
<img src="https://github.com/pil0706/pil0706.github.io/blob/master/screenshots/positionofpois/apple_eu_z3z4_overlap_again.png?raw=true"> | <img src="https://github.com/pil0706/pil0706.github.io/blob/master/screenshots/positionofpois/apple_eu_z4z5_overlap_withdots.png?raw=true">





### How The Label Positions are Different in Google Maps and Apple Maps


Now, it is obvious that the label positions of Apple Maps and Google Maps are very different.
One stays in same position and the other hops in each level.
<br>
<br>
I overlapped Apple and Google maps again.<br>
The two Koreas' label positions are somewhat similar.<br>
Difference between Apple and Google maps is just linebreak.
<br>
<br>
But, Google and Apple seemed to focus more in Japan,<br>
Because, JAPAN (in Apple) and Japan (in Google) are in different spots
<br>
<br>
In Apple Maps, JAPAN is very closed to Sendai; on the other hand, Japan stays in Honshu, the main island.
<br>
<br>
<img src="https://github.com/pil0706/pil0706.github.io/blob/master/screenshots/positionofpois/z6asia_label_sq.png?raw=true">

I know Apple does not pay too much attention to Korean market.<br>
I also know Google is trying to expand its territory to South Korea but the government puts regulation on Google.<br>

> the two koreas are abandoned by the two companies.

<br>
<br>
Japan, however, is important market in Asia and I know the two companies are paying much attention on it compare to Koreas
<br>
<br>
Let's go to Europe again
<br>
<br>
<img src="https://github.com/pil0706/pil0706.github.io/blob/master/screenshots/positionofpois/z6eu_label_sq.png?raw=true">
<br>
Europe, because of its lable density, is the best place to compare label positions.
<br>
<br>
Other than France, most of 'well-known' European countries label positions are different in the two services.
<br>
But countries like Romania, Bulgaria, Moldova, Slovenia, Austria, Hungary, Switzerland, etc.,<br>
In Apple Maps and Google Maps, the label positions are almost overlapped.
<br>
<br>
What I can guess is that
- if the two maps label positions are close enough,
    - means that they are not paying much attention? (except, France?)
- else,
    - they are being cared?
<br>
<br>
Apple and Google Maps only know.<br>
But, I know for sure that the two Koreas are not being focused.<br>
<br>
<br>
From the screenshots above, you now can tell the two services have totally different philosophies in map designing.

### What about Capitals?

It seems like Google Maps considers capital cities when country lables are plotted.
<br>
For instance, the centroid of Poland is south-west area of its capital, Warsaw.<br>
But, Google moved it up of Warsaw so that it does not overlapped as much as it was before.
<br>
If it stays in centroid of the country, and it covers the capital, either one of labels will not be shown.

<img src="https://github.com/pil0706/pil0706.github.io/blob/master/screenshots/positionofpois/ne_centroid_z5_eu1.png?raw=true">

<br>
<br>
<br>
<br>
Also, I have noticed that if there aren't enough space to move the labels (like Belgium & the Nerherlands),<br>
Google decided to reduce the font size based on its area.

<img src="https://github.com/pil0706/pil0706.github.io/blob/master/screenshots/positionofpois/ne_centroid_z5_eu2.png?raw=true">

One funny thing is Belarus is very Big country though the label is smaller than its neighbors
<br>
<br>
<br>
<br>
These, I guess, are the rule of thumb in POI and Label positioning areas. (The ZLv follows Google's ZLv)

- Zoom Lv 3, where capitals can be shown if there are enough spaces, country labels are more important than the capital labels
- Zoom Lv 4, it might be nice to show "well-known" capitals such as Paris, London, Berlin, Oslo, Rome, etc.
- Zoom Lv 5, capitals are better be on even if cartographers adjust the country label's original position.
- Zoom Lv 6, capitals must be exposed unless city countries like Singapore, Vatican City, Monaco, and so on.
- from Zoom Lv 7, I don't have to mention.

<br>
<br>
Keep those in your mind, and let's go back to the Portugal's example.

<img src="https://github.com/pil0706/pil0706.github.io/blob/master/screenshots/positionofpois/google_z_portugal.gif?raw=true">

Lisbon, the capital, does not really need to be shown in Zoom Lv 3.<br>
Lisbon is not as big as Madrid (no offense to Portuguese) so Google Maps seems to decide to show more well-known cities than Lisbon.<br>
<br>
<br>
But, the label of Portugal is moved up for the next Zoom Lv<br>

> by moving around the labels, cartographers can reduce the risks of map readers gets 'surprised' when lots of cities are on in next zoom level

<br>
When the capital and the country label are taking stable positions, where no other labels are interrupted such as from Zlv 5 - 6, they remain in same position.
<br>
<br>
What about Apple Maps?
<br>
<br>
I positioned the label of Portugal in center as much as possible.


<img src="https://github.com/pil0706/pil0706.github.io/blob/master/screenshots/positionofpois/apple_z_portugal.gif?raw=true">


Yes, Portugal never changes.<br>
Also, other country labels never changes it's position.

> We've checked this above

Therefore, Warsaw is hidden by Poland, in which you do not see on Google Maps.<br>
Warsaw is showed up at the last as I zooming in, though it's the capital.<br>

> I suppose the Map App. calculates the collision of the labels in client side.

<img src="https://github.com/pil0706/pil0706.github.io/blob/master/screenshots/positionofpois/Apple_Warsaw.png?raw=true">

<br>
<br>
I have also noticed that Apple Maps is following conventional rules of cartography, such as labeling as much as possible.<br>
<br>
You may also find it from National Geographic Maps.
<br>
<br>
Apple Maps is going harder way, for country labels should be in "optimal" location where it considers its neighbor country labels and capital labels (even sometimes well-known cities).
<br>
<br>
I have never heard of automating label position tools.<br>
Lower zoom levels of Web-Map are areas where machines cannot create aesthetic balance, for it has so much consideration. (Google may be..?)
<br>
<br>
Google Maps' label hopping is more rational for cartographers like me,<br>
because I can manually adjust most optimal location of them level by level.<br>

> there are only 200 something countries and 200 something capitals, it is not much hassles to me.

Something came up to my mind that Apple might not have a function to support a tool like Google has.
<br>
<br>
If you are working for a cartographer, you would know what I meant.
For those who are not familiar, let me explain.
<br>
Usually, a label on a map is one record in a table. ~(it sounds like 'ship shipping ship shipping shipping ships')~<br>
<br>
<br>
When lable has to hop like Google, a label is duplicates but not in geometry perspectives. (though it might have Zlv in fields)<br>
<br>
<br>
What I can assume is Google has multiple records of coutries or they have a VERY NICE tool to control all that.
<br>
<br>
On the other hand, Apple might not.<br>
In this case, they should keep only one table and make very precise initial position.
<br>
<br>
I would make multiple tables and pop the label positions like Google ~(still doesn't know Google uses multiple tables though)~<br>
I will find them out someday.
<br>
<br>
<br>
<br>
By the way, I should write an article of National Geographic Labeling and Label's priority rule someday.
<br>
<br>
<br>
<br>
PS1 : There are diplomatic issues between Japan and Korea. <br>
I do not want my lovely countries are fighting. But I saw something bizarre in Seoul.<br>
- Apple Maps in デモ
Hey, come on...<br>
You really think Embassy's priority is that high in that zoom level?

<img src="https://github.com/pil0706/pil0706.github.io/blob/master/screenshots/positionofpois/japanese_embassy.png?raw=true">

I don't like Maps are being used to cause political controversial.
<br>
<br>
<br>
<br>
<br>
PS2 : I reall do want to know what tools Google uses and how they make maps.<br>
- Copenhagen Pikabu

<img src="https://github.com/pil0706/pil0706.github.io/blob/master/screenshots/positionofpois/copenhagen_pikabu.png?raw=true">

As soon as Denmark is gone, Copenhagen popped up.<br>
PIKA.....BU!!!!!
<br>
<br>

--- 한국어 버전