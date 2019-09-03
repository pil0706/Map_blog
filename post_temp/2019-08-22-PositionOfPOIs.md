---
layout: post
title: Popping Labels : Map Label Placement - Copenhagen Pikabu | 뛰어 다니는 레이블(주기) : 지도 레이블(주기) 위치 - 코펜하겐 까꿍
---

# Label, the Finale of Cartography

Because of limited space,
it is always hard to show all the labels on a map.


Let's say you are in a situation of labeling names of countries, especially in a lower zoom level.


Each one of labels are very important.
If a country's label is hided or overlapped by another country's, someone might be upset.


Therefore, cartographers must choose what to show or where to locate labels under a clear policy.


One day,
One of my colleagues asked me, can a label of Portugal be shown in low zoom level.


For instance, adjacent countries, Spain and Portugal,
Portugal might not show up, for Spain takes space.
In other words, there is no enough space to pose the label of Portugal.

<img src="https://github.com/pil0706/pil0706.github.io/blob/master/screenshots/positionofpois/no_portu.png?raw=true">


If I were a Portuguese, I might be upset.

However, if the cartographer is Spanish?
Spain comes first than Portugal, for his sake.


To not to get egged, I see that Google Maps adjusts the labels in each zoom level.

<img src="https://github.com/pil0706/pil0706.github.io/blob/master/screenshots/positionofpois/portu_location_change.gif?raw=true">

From Zoom Lv5, it seems like the label keeps its position till it gets dissapeared.

On the other hand, Apple Maps does seem to change labels location.

<img src="https://github.com/pil0706/pil0706.github.io/blob/master/screenshots/positionofpois/portu_location_change_apple.gif?raw=true">


Apple Maps keeps their lable position consistently; on the other hand, Google Maps is more flexible in their label position.


Based on my almost 9 years of map making experiences, it's very obvious that Apple and Google adjust unmovable labels manually.
> I just coined out the term 'unmovalbe labels'. Unmovable Lables can be defined as labels of countries, cities, airport, etc.

I can tell they are not using centroid of each countries.

I used 'Centroid on Surface' to have center points of each countries.
Here, I drew arrows between countries' centroid and Google's label.

<img src="https://github.com/pil0706/pil0706.github.io/blob/master/screenshots/positionofpois/naturalearth_google.gif?raw=true">


The reason why I am showing this is that I want to emphasize Google and Apple did not just use simple centroid for labeling but **someone** (and I strongly believe that he or she is a very well cartographer who carries Google and Apple's internal policies or philosophies) manually replotted them.

<img src="https://github.com/pil0706/pil0706.github.io/blob/master/screenshots/positionofpois/ne_google_z4.png?raw=true">


Google changes their location level by level, on the other hand
Apple sets its initial location and uses all zoom levels

Here, it took me forever to capture Apple Maps level by level

<img src="https://github.com/pil0706/pil0706.github.io/blob/master/screenshots/positionofpois/apple_google_z4.png?raw=true">

> I tried to match Apple's Zoom level to Google's Zoom Level but this was the best I could do.


<img src="https://github.com/pil0706/pil0706.github.io/blob/master/screenshots/positionofpois/apple_google_overlap.png?raw=true">


I re-sized (reduced) Apple Maps Zoom level 5.

<img src="https://github.com/pil0706/pil0706.github.io/blob/master/screenshots/positionofpois/apple_eu_z3z4_overlap_again.png?raw=true">


To improve the readability of label's location, I dotted the center of labels in Europe.


Although I pointed my shaking hands and PowerPoint's auto snapping, the lables position remained almost in same spots.

Z3-Z4 | Z4-Z5
-- | --
<img src="https://github.com/pil0706/pil0706.github.io/blob/master/screenshots/positionofpois/apple_eu_z3z4_overlap_again.png?raw=true"> | <img src="https://github.com/pil0706/pil0706.github.io/blob/master/screenshots/positionofpois/apple_eu_z4z5_overlap_withdots.png?raw=true">





# How The Label Positions are Different


It is obvious that the label positions of Apple Maps and Google Maps are very different.

the two Koreas' label positions are somewhat similar. Difference between Apple and Google is just linebreak.

But Google and Apple seemed to focus more in Japan.
Because, there label positions are different in two maps.


Japan's label position is very closed to Sendai area in Apple; on the other hand, Japan in Google stays in Honshu, the main island.

<img src="https://github.com/pil0706/pil0706.github.io/blob/master/screenshots/positionofpois/z6asia_label_sq.png?raw=true">

I know Apple does not pay too much attention to Korean market.
I also know Google is trying to expand its territory to South Korea but the government puts regulation on Google.
So the two koreas are abandoned by the two companies.

Japan, however, is very important market in Asia and I know the two companies are paying much attention on it.



Let's go to Europe and see

<img src="https://github.com/pil0706/pil0706.github.io/blob/master/screenshots/positionofpois/z6eu_label_sq.png?raw=true">

I noticed that Europe was the best place where I can compare labels easily, for countries are very clustered.

It might be my stereotypes. Or I maybe don't know much about Europe. Other than France, most of 'well-known' European countries label positions are different in the two services.

But the other countries, such as Romanica, Bulgaria, Moldova, Slovenia, Austria, Hungary, Switzerland, etc., I know there markets are not big enough nor population either.

What I can guess is that
- if the two services' label positions are close enough
    - then, the two services are not paying much attention?
- else,
    - they are special?

Cartographers in Apple Maps and Google Maps only know the facts.
But, I know for sure that the two services' maps in the two Koreas are no good at all.

From the screenshots above, you now can tell the two services have totally different philosophies in map designing.








# What about Capitals?


It seems like Google Maps also considered capital cities together when country lables are plotted.


For instance, the centroid of Poland is south-west area of its capital, Warsaw.
But, Google moved it up of Warsaw so that it does not overlapped as much as it was before.

If it stays in centroid of the country, and it covers the capital, either one of labels will not be shown.

<img src="https://github.com/pil0706/pil0706.github.io/blob/master/screenshots/positionofpois/ne_centroid_z5_eu1.png?raw=true">

Also, I have noticed that if there aren't enough space to move the labels (like Belgium & the Nerherlands), Google decided to reduce the font size based on its area.

<img src="https://github.com/pil0706/pil0706.github.io/blob/master/screenshots/positionofpois/ne_centroid_z5_eu2.png?raw=true">

One funny thing is Belarus is very Big country though the label is smaller than its neighbors







I see Google cared in label position in every zoom levels.

This, I guess, is the rule of thumb in POI and Label positioning areas.

- Zoom Lv 3, where capitals can be shown if there are enough spaces, country labels are more important than the capital labels
- Zoom Lv 4, it might be nice to show "well-known" capitals such as Paris, London, Berlin, Oslo, Rome, etc.
- Zoom Lv 5, capitals are better be on even if cartographers adjust the country label's original position.
- Zoom Lv 6, capitals must be exposed unless city countries like Singapore, Vatican City, Monaco, and so on.
- from Zoom Lv 7, I don't have to mention.


Let's go back to the Portugal's example.


<img src="https://github.com/pil0706/pil0706.github.io/blob/master/screenshots/positionofpois/google_z_portugal.gif?raw=true">

Lisbon, the capital, does not really need to be shown in Zoom Lv 3.
Lisbon is not as big as Madrid (no offense to Portuguese) so Google Maps seemed to decide more well-known cities than Lisbon. But, the label of Portugal is moved for the next Zoom Lv
> by moving around the labels, cartographers can reduce the risks of map readers gets 'surprised' when lots of cities are on in next zoom level
When the capital and the country label are taking stable positions, where no other labels are interrupt, they remain in same position.


What about Apple Maps?


I positioned the label of Portugal in center as much as possible.


<img src="https://github.com/pil0706/pil0706.github.io/blob/master/screenshots/positionofpois/apple_z_portugal.gif?raw=true">


Yes, Portugal never changes. Also, other country labels never changes it's position.



Therefore, Warsaw is hidden by Poland, in which you do not see on Google Maps, and ended up showing the last compared to other cities in Poland when zooming-in.

> I suppose the Map App. calculates the collision of the labels in client side.

<img src="https://github.com/pil0706/pil0706.github.io/blob/master/screenshots/positionofpois/Apple_Warsaw.png?raw=true">


I have also noticed that Apple Maps is following conventional rules of cartography, such as labeling as much as possible.
You may also find it from National Geographic Maps.




I think Apple Maps is going harder way, for country labels should be in "optimal" location where it considers its neighbor country labels and capital labels.


I have never heard of automating label position tools.
Lower zoom levels of Web-Map are areas where machines cannot create aesthetic balance, for it has so much consideration. (Google may be..?)



Google Maps' label hopping is more rational for cartographers like me, because I can adjust most optimal location of them level by level.

> there are only 200 something countries and 200 something capitals, it is not much hassles to me.



Something came up to my mind that Apple might have a tool to support a tool like Google has.

If you are working for a cartographer, you would know what I meant.
For those who are not familiar, let me explain.

Usually, a point stays one position and it becomes a label on a map.
When lable has to pop like Google, a point should have multiple positions.
What I can assume is Google has multiple tables of coutry labels for each level or they have a VERY NICE tool to control all that.

On the other hand, Apple might not. In this case, they should keep only one table and make very precise initial position.


I would make multiple tables and pop the label position like Google (still doesn't know Google uses multiple tables though)




Maybe, I should write an article of National Geographic Labeling and Label's priority rule someday.





PS1 : There are diplomatic issues between Japan and Korea. I do not want my lovely countries are fighting. But I saw something bizarre in Seoul.
- Apple Maps in デモ

Hey, come on...
You really think Embassy's priority is that high in that zoom level?

<img src="https://github.com/pil0706/pil0706.github.io/blob/master/screenshots/positionofpois/japanese_embassy.png?raw=true">


I don't like Maps are being used to cause political controversial.


PS2 : I reall do want to know what tools Google uses and how they make maps.
- Copenhagen Pikabu

<img src="https://github.com/pil0706/pil0706.github.io/blob/master/screenshots/positionofpois/copenhagen_pikabu.png?raw=true">

As soon as Denmark is gone, Copenhagen popped up.
PIKA.....BU!!!!!


--- 한국어 버전