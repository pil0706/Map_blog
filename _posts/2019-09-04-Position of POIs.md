---
layout: post
title: Hopping Labels | 뛰어 다니는 주기
---

## It's all about, Label Placement.

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
For instance, adjacent countries like Spain and Portugal.<br>
Portugal might not show up, for Spain takes space.<br>
In other words, there is no enough space to pose the label of Portugal in Iberia penninsula.
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
On the other hand, Apple Maps does not seem to change labels location.
<br>
<br>
<img src="https://github.com/pil0706/pil0706.github.io/blob/master/screenshots/positionofpois/portu_location_change_apple.gif?raw=true">
<br>
<br>
Apple Maps keeps their lable position consistently; on the other hand, Google Maps is more flexible in their label position.
<br>
<br>
Based on my almost 9 years of map making experiences, it's obvious that Apple Maps and Google Maps adjust **the place labels** manually.

> the place lables can be defined as labels of countries, cities, airport, etc.

I can tell they are not using centroid of each countries.
<br>
I used 'Centroid on Surface' to show center points of each countries, <br>
and drew lines between centroid points of each contries from Natural Earth data and Google Maps place labels.
<br>
<br>

<img src="https://github.com/pil0706/pil0706.github.io/blob/master/screenshots/positionofpois/naturalearth_google.gif?raw=true">

<br>
<br>
The reason why I am showing this is that<br>
I want to emphasize Google Maps and Apple Maps did not just use simple centroid for labeling<br>
<br>
And, **someone** (and I strongly believe that he or she is a very well trained cartographer who carries Google and Apple's internal policies or philosophies) manually replotted the lables.
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

> I tried to match Apple's Zoom level to Google's Zoom Level but the screenshot above was the best I could do.

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
With my shaking hands and PowerPoint's auto snapping, I was able to know that the lables position remained almost in same spots in every levels in Apple Maps.

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
In Apple Maps, JAPAN is very closed to Sendai; on the other hand, in Google Maps, Japan stays in Honshu, the main island.
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
Other than France, most of 'well-known' European countries' label positions are not located in the center of the countries.
<br>
Meanwhile, In Apple Maps and Google Maps,<br>
countries like Romania, Bulgaria, Moldova, Slovenia, Austria, Hungary, Switzerland, etc.,<br>
the label positions are almost overlapped.
<br>
<br>
What I can guess is that<br>
- if a country's label position in the two maps are close enough,
    - means that, the country is not being focused by Apple and Google Maps(except, France?)
- else,
    - it is being cared?

<br>
<br>
But, I know for sure that the two Koreas are not being focused.<br>
From the screenshots above, you now can tell the two services have totally different philosophies in map designing.

### What about Capitals?

It seems like Google Maps considers capital cities when country lables are plotted.
<br>
For instance, the centroid of Poland is south-west area of its capital, Warsaw.<br>
But, Google moved the country label up of Warsaw so that it does not overlapped with the capital.
<br>
If it stays in centroid of the country, and it covers the capital, either one of labels will not be shown.

<img src="https://github.com/pil0706/pil0706.github.io/blob/master/screenshots/positionofpois/ne_centroid_z5_eu1.png?raw=true">

<br>
<br>
Also, I have noticed that if there aren't enough space to move the labels (like Belgium & the Nerherlands),<br>
<br>
Google decided to reduce the font size based on its area.

<img src="https://github.com/pil0706/pil0706.github.io/blob/master/screenshots/positionofpois/ne_centroid_z5_eu2.png?raw=true">

One funny thing is Belarus is very Big country though the label is smaller than its neighbors
<br>
<br>
<br>
<br>
These, I guess, are the rule of thumb in POI and Label positioning.<br>
(The ZLv follows Google's ZLv)

- Zoom Lv 3, where capitals can be shown if there are enough spaces, <br>     - country labels are more important than the capital labels
- Zoom Lv 4, it might be nice to show "well-known" capitals <br>
    - such as Paris, London, Berlin, Oslo, Rome, etc.
- Zoom Lv 5, capitals are better be on <br>
    - even if cartographers adjust the country label's initial position.
- Zoom Lv 6, capitals must be exposed<br>
    - except city countries like Singapore, Vatican City, Monaco, and so on.
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

> by moving around the labels, cartographers can reduce the risks of map readers gets 'surprised' when lots of cities are popped in next zoom level

<br>
When the capital and the country label are taking stable positions, where no other labels are interrupted such as from Zlv 5 - 6, they remain in same position.
<br>
<br>
What about Apple Maps?
<br>
<br>
I positioned the label of Portugal in center of the screen.


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

Something came up to my mind that Apple might not have a tool to place lables like Google has.
<br>
<br>
If you are working for a cartographer, you would know what I meant.<br>
For those who are not familiar, let me explain.
<br>
Usually, a label on a map is one record in a table. <br>
<br>
<br>
When lable has to hop like Google, a label is duplicates but not in geometry perspectives. (though it might have Zlv in fields)<br>
<br>
<br>
What I can assume is Google has multiple records of a country or they have a VERY NICE tool to control all that.
<br>
<br>
On the other hand, Apple might not.<br>
In this case, they might keep only one record of a country and make very precise initial position.
<br>
<br>
I would make multiple records and pops the label positions like Google<br>
(still doesn't know Google uses multiple tables though)<br>
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
PS1 : デモ in Apple Maps<br>
<br>
There are diplomatic issues between Japan and Korea. <br>
I do not want my lovely countries are fighting. But I saw something bizarre in Seoul.<br>
<br>
Hey, come on...<br>
You really think Embassy's priority is that high in that zoom level?

<img src="https://github.com/pil0706/pil0706.github.io/blob/master/screenshots/positionofpois/japanese_embassy.png?raw=true">

I don't like Maps are being used to cause political controversial.
<br>
<br>
<br>
<br>
<br>
PS2 : Copenhagen Pikabu<br>
<br>
I really do want to know what tools Google uses and how they make maps.<br>

<img src="https://github.com/pil0706/pil0706.github.io/blob/master/screenshots/positionofpois/copenhagen_pikabu.png?raw=true">

As soon as Denmark is gone, Copenhagen popped up.<br>
PIKA.....BU!!!!!
<br>
<br>






--- 한국어 버전






## 이 모든것은 주기 배치이다.

### Cartography의 피날레, 주기

제한된 공간으로 인해, <br>
지도위에 모든 주기를 보여주는것은 항상 어렵습니다.
<br>
<br>
당신이 국가 이름의 주기를 배치해야하는 상황에 있다고 가정합니다,
특별히, 낮은 줌 레벨에서
<br>
<br>
각각의 주기는 매우 중요합니다.<br>
만약의 한 나라의 주기가 다른 나라의 것으로 가려지거나, 겹처지게 된다면, 누군가는 화가날지도 모릅니다.
<br>
<br>
그러므로, Cartographers는 분명한 정책의 아래에서 반드시 선택해야합니다, 무엇을 보여주고 어디에 위치시켜야할지를.
<br>
<br>
어느날,<br>
저의 동료중 한명이 저에게 질문을 했습니다, 포루투갈의 주기를 낮은 줌 레벨에서 보일 수 있겠는지.
<br>
<br>
예를들어, 스페인과 포루투갈처럼 이웃한 나라.<br>
스페인이 공간을 차지하고 있기 때문에, 포루투갈이 안나올 수 있습니다.
다른말로 하자면, 포루투갈 주기를 놓을 공간이 이베리아 반도에는 없습니다.
<br>
<br>
<img src="https://github.com/pil0706/pil0706.github.io/blob/master/screenshots/positionofpois/no_portu.png?raw=true">
<br>
<br>
제가 만약 포루투갈 사람이라면, 화가 났을지도 모릅니다.
<br>
하지만, 만약 Cartographer가 스페인사람이라면?<br>
스페인이 포루투갈보다 먼저 나오게 될 것입니다.
<br>
<br>
계란을 맞지 않으려고, 구글 지도는 각 줌 레벨별로 주기를 조절한게 보인다.
<br>
<br>
<img src="https://github.com/pil0706/pil0706.github.io/blob/master/screenshots/positionofpois/portu_location_change.gif?raw=true">
<br>
<br>
줌 레벨 5 부터, 주기가 없어질때까지 그 자리를 지키는것처럼 보입니다.
<br>
반면에, 애플 지도는 주기의 위치가 변하지 않는것처럼 보입니다.
<br>
<br>
<img src="https://github.com/pil0706/pil0706.github.io/blob/master/screenshots/positionofpois/portu_location_change_apple.gif?raw=true">
<br>
<br>
애플 지도는 그들의 주기 위치를 꾸준하게 유지합니다; 반면에, 구글 지도는 그들의 주기 위치를 좀 더 유연하게 합니다.
<br>
<br>
저의 9년간의 지도 제작 경험을 기반으로, 애플 지도와 구글 지도는 **the place 주기**를 수작업으로 조절하는것이 분명합니다.

> the place 주기는 나라, 도시, 공항 등의 주기로 정의 될 수 있다.

확실한것은, 그들은 각 국가의 centroid 를 사용하지 않는것 입니다.

<br>
저는 'Centroid on Surface'를 사용하여 각 국가의 중심점을 표현하고, <br>
Natural Earth 데이터로부터의 중심점과 구글 지도의 주기 사이를 연결했습니다.
<br>
<br>

<img src="https://github.com/pil0706/pil0706.github.io/blob/master/screenshots/positionofpois/naturalearth_google.gif?raw=true">

<br>
<br>
제가 이것을 보여주는 이유는<br>
구글 지도와 애플지도가 단순히 중심점을 주기의 위치로 사용하지 않았음을 강조하기 위해서 이고<br>
<br>
그리고, **누군가** (그리고 저는 강하게 믿습니다, 그/그녀가 구글과 애플의 내부 정책 혹은 철학을 수행하는 잘 훈련된 Cartographers라고) 가 수작업으로 다시 주기를 찍었음을.
<br>
<br>

<img src="https://github.com/pil0706/pil0706.github.io/blob/master/screenshots/positionofpois/ne_google_z4.png?raw=true">
<br>
<br>

또한, 구글 지도는 주기의 위치를 레벨 별로 변화 합니다.<br>
반면에, 애플 지도는 처음 주기의 위치를 모든 줌 레벨에서 사용합니다.
<br>
<br>

<img src="https://github.com/pil0706/pil0706.github.io/blob/master/screenshots/positionofpois/apple_google_z4.png?raw=true">

> 저는 애플 지도의 줌 레벨을 구글 지도의 줌 레벨과 맞추기 위해 노력을 했고, 위 스크린샷이 제가 최선을 한 결과 입니다.

<img src="https://github.com/pil0706/pil0706.github.io/blob/master/screenshots/positionofpois/apple_google_overlap.png?raw=true">
<br>

> 그리고 마침내 애플 지도와 구글 지도를 같은 축척으로 맞추었습니다


<br>
<br>
저는 애플 지도의 줌 레벨3과 줌 레벨4의 국가 주기의 중심을 마크했습니다.
<br>
그리고, 애플 지도의 국가 주기의 위치를 비교하기위해, 줌 레벨4를 줌레벨 3과 맞추기 위해 크기를 조절하였습니다.


<img src="https://github.com/pil0706/pil0706.github.io/blob/master/screenshots/positionofpois/apple_eu_z3z4_overlap_again.png?raw=true">

<br>
<br>
나의 떨리는 손으로 그리고 파워포인트의 자동 스냅핑으로, 저는 애플 지도에서 확인할 수 있었습니다. 주기의 위치는 모든 레벨에서 거의 똑같은 위치에 있었음을


Z3-Z4 | Z4-Z5
-- | --
<img src="https://github.com/pil0706/pil0706.github.io/blob/master/screenshots/positionofpois/apple_eu_z3z4_overlap_again.png?raw=true"> | <img src="https://github.com/pil0706/pil0706.github.io/blob/master/screenshots/positionofpois/apple_eu_z4z5_overlap_withdots.png?raw=true">





### 구글 지도와 애플 지도에서 어떻게 주기의 위치가 다른가


이제, 이것은 명확해졌습니다. 애플 지도와 구글 지도에서의 주기 위치는 매우 다르다는것을.
애플은 하나의 위치에 머무르고, 구글은 각 레벨에서 뛰어 다니는 것을.
<br>
<br>
저는 애플 지도와 구글 지도를 다시 겹쳤습니다.<br>
두 서비스에서 두개의 한국들(한국/북한)의 주기 위치는 어쩌면 비슷합니다.<br>
애플 지도와 구글 지도의 차이점은 그냥 개행입니다.
<br>
<br>
하지만, 구글 지도와 애플 지도는 일본에 더 관심을 두는 듯 해 보입니다.<br>
왜냐하면, JAPAN (애플 지도의) 과 Japan (구글 지도의) 의 위치가 다르기 때문입니다.
<br>
<br>
애플 지도에서 JAPAN은 센다이 지역과 가깝습니다; 반면에, 구글의 Japan은 혼슈 섬에 머물러 있습니다.
<br>
<br>
<img src="https://github.com/pil0706/pil0706.github.io/blob/master/screenshots/positionofpois/z6asia_label_sq.png?raw=true">

저는 알고 있습니다. 애플 지도가 한국 시장에 크게 관심을 두고 있지 않음을.<br>
저는 또한 알고 있습니다, 구글 지도가 한국 시장으로 넓혀 가고 싶지만 한국 정부가 그것을 규제하고 있음을.<br>

> 두개의 한국 (한국/북한)은 두 회사에 의해 버려졌습니다.

<br>
<br>
하지만, 일본은 아시아에서 매우 중요한 시장입니다 그리고 두 회사는 한국에 비해 더 많은 관심을 일본에 두고 있습니다.
<br>
<br>
다시 유럽으로 갑니다.
<br>
<br>
<img src="https://github.com/pil0706/pil0706.github.io/blob/master/screenshots/positionofpois/z6eu_label_sq.png?raw=true">
<br>
주기의 밀도 때문에, 유럽은 주기 위치를 비교하기에 매우 좋은 곳 입니다.
<br>
<br>
프랑스를 제외하고, 왠만큼 잘 알려진 유럽 국가의 주기들은 국가 중심점에 있지 않습니다.
<br>
한편, 애플 지도와 구글 지도에서<br>
루마니아, 불가리아, 몰도바, 슬로베니아, 오스트리아, 헝그리, 스위스 등<br>
주기의 위치가 거의 겹칩니다.
<br>
<br>
제가 추측할 수 있는 것은<br>
- 만약 한 나라의 주기 위치가 두 서비스에서 충분히 가깝다면,
    - (프랑스를 제외하고?) 그 국가는 관심 받지 못하는 국가이고
- 그렇지 않으면,
    - 관심을 받고 있나?

<br>
<br>
하지만, 저는 확실히 알고있습니다, 두개의 한국은 관심받고 있지 않음을<br>
위 스크린샷으로 부터, 두개의 서비스는 지도 디자인에 완전히 다른 철학을 갖고 있음을 당신은 이제 알고 있습니다.

### 수도는 어떻게?

구글 지도는 국가 주기를 놓을 때 수도를 고려하는것처럼 보입니다.
<br>
예를 들어, 폴란드의 중심은 바르샤바의 남서쪽에 위치하고 있습니다.<br>
하지만, 구글 지도는 국가 주기를 바르샤바의 윗쪽으로 이동하여 수도와 겹치지 않게 했습니다.
<br>
만약 국가 주기가 폴란드의 중심에 머물게 된다면, 이것은 수도를 가리게 되거나 두개중 하나의 주기는 보여지지 않을 것 입니다.

<img src="https://github.com/pil0706/pil0706.github.io/blob/master/screenshots/positionofpois/ne_centroid_z5_eu1.png?raw=true">

<br>
<br>
또한, 벨기에와 네덜란드처럼 주기를 옮길 수 없는 충분한 공간이 없음을 확인했습니다.<br>
<br>
이때, 구글 지도는 그들의 면적을 고려하여 폰트 크기를 줄이도록 결정했습니다.

<img src="https://github.com/pil0706/pil0706.github.io/blob/master/screenshots/positionofpois/ne_centroid_z5_eu2.png?raw=true">

하나 재미있는 것은, 벨라루스는 면적이 큰 국가이지만 주기는 그 이웃들보다 작았습니다.
<br>
<br>
<br>
<br>
이것들은 제가 추측하건데 POI와 주기 위치의 경험적인 규칙입니다.<br>
(줌 레벨은 구글의 줌 레벨을 따릅니다.)

- 줌 레벨 3, 만약 충분한 공간이 있으면 수도는 보여집니다 <br>
    - 국가 주기는 수도 주기보다 더 중요합니다
- 줌 레벨 4, 잘 알려진 수도를 표현하는것은 좋습니다 
    - 가령, 파리, 런던, 베를린, 오슬로, 로마 등
- 줌 레벨 5, 수도는 보여지는게 좋습니다
    - Cartographers가 국가 주기의 처음 위치를 조절하더라도
- 줌 레벨 6, 수도는 반드시 노출되어야 합니다 
    - 싱가폴, 바티칸, 모나코 등 국가 도시 등을 제외하고
- 줌 레벨 7 부터, 말할 필요 없습니다

<br>
<br>
이것들을 마음에 두고, 다시 포루투갈의 예시로 갑니다.

<img src="https://github.com/pil0706/pil0706.github.io/blob/master/screenshots/positionofpois/google_z_portugal.gif?raw=true">

수도인 리스본은 줌 레벨 3에서 보여질 필요가 없습니다.<br>
리스본은 마드리드 만큼 크지 않습니다 (포루투갈 사람들 미안합니다). 그래서 구글 지도는 리스본 보다 더 유명한 것을 보여주려고 결정하였습니다.<br>
<br>
<br>
하지만, 포루투갈의 주기는 다음 줌 레벨에서 위로 옮겨집니다<br>

> 주기를 움직여서, Cartographers는 갑자기 많은 도시가 다음 레벨에서 나타날 때 깜짝 놀랄 수 있는 위험을 줄일 수 있습니다.

<br>
국가와 수도의 주기가 다른 주기로부터 방해받지 않는 (예를 들면 줌 레벨 5 - 6)안정적인 위치에 있으면, 그들은 같은 위치에 남아있습니다.
<br>
<br>
애플 지도는 어떤가요?
<br>
<br>
저는 포루투갈의 주기를 화면 중심에 고정시켰습니다.


<img src="https://github.com/pil0706/pil0706.github.io/blob/master/screenshots/positionofpois/apple_z_portugal.gif?raw=true">


네, 포루투갈은 전혀 변하지 않습니다.<br>
또한, 다른 국가의 주기도 그것들의 위치를 바꾸지 않습니다.

> 우리는 위에서 이것을 확인했습니다.

따라서, 바르샤바는 폴란드에의해 가려집니다, 구글 지도에서는 볼 수 없습니다.<br>
바르샤바는 제가 줌인을 할 때 비로소 마지막에 나타납니다.<br>

> 아마 지도 어플리캐이션이 주기의 충돌을 계산하는 것 같습니다.

<img src="https://github.com/pil0706/pil0706.github.io/blob/master/screenshots/positionofpois/Apple_Warsaw.png?raw=true">

<br>
<br>
저는 또한 확인했습니다. 애플 지도는 과거의 Cartography의 규칙을 따르는것을, 예를 들면 주기를 최대한 많이 넣는것.<br>
<br>
내셔널 지오그래픽 지도에서 이런것을 찾을 수 있습니다.
<br>
<br>
애플 지도는 어려운 길을 가고 있습니다. 왜냐하면 국가 주기는 이웃 국가와 수도를 고려하여 최적의 장소에 위치해야 하기 때문입니다.
<br>
<br>
저는 주기 위치를 자동으로 위치하는 도구를 들은적이 없습니다.<br>
웹 지도의 낮은 줌 레벨은 고려할 것이 많기에 기계가 심미적인 균형을 맞추기 어렵습니다 (구글은 어쩌면..?)
<br>
<br>
구글 지도의 뛰어다니는 주기는 저 와 같은 Cartographers에겐 좀 더 이성적으로 보입니다<br>
왜냐하면, 저는 수작업으로 각 레벨 별로 최적의 주기 위치를 배치할 수 있습니다.<br>

> 약 200개의 국가와 200개의 수도를 배치하는것은 저에게 그리 어려운 일은 아닙니다.

애플 지도는 어쩌면 구글 지도와 같은 주기 배치 도구가 없는것이 아닐까?라는 생각이 들었습니다.
<br>
<br>
만약 당신이 Cartographer라면 제가 무슨말을 하는지 알 것 입니다.<br>
익숙하지 않은 분들을위해 설명드리겠습니다.
<br>
일반적으로, 지도의 주기는 DB테이블의 하나의 레코드입니다<br>
<br>
<br>
구글 지도 처럼 주기가 뛰어 다니려면, 주기의 위치가 다른 중복 레코드가 필요합니다 (하지만, 줌레벨에 따라 선택할 수 있는 필드가 필요합니다)<br>
<br>
<br>
제가 추측할 수 있는 것은 구글은 어쩌면 엄청 좋은 도구를 갖고 있어 이 모든것을 컨트롤 하거나, 아니면 하나의 국가에 대해 줌레벨별 중복 레코드가 있습니다.
<br>
<br>
반면에 애플은 아닐지도 모릅니다.<br>
이 경우라면, 애플은 주기를 하나의 레코드에 저장하지만, 최초의 위치를 매우 정교하게 만들었습니다.
<br>
<br>
저는 구글처럼 뛰어다니는 주기를 만들기 위해 여러개의 레코드를 만들겠습니다.<br>
(구글이 중복 레코드를 사용하는지 아닌지는 모릅니다)<br>
언젠가 확인하겠습니다.
<br>
<br>
<br>
<br>
그나 저나, 언젠가 내셔널 지오그래픽의 주기와 주기 우선순위 규칙에 대해 글을 써봐야 하겠습니다.
<br>
<br>
<br>
<br>
PS1 : 애플 지도의 데모<br>
<br>
일본과 한국사이 외교 문제가 있습니다.<br>
나의 사랑하는 나라들이 싸우는걸 바라지 않습니다.
하지만 저는 서울에서 이상한것을 봤습니다.<br>
<br>
이봐요...<br>
대사관의 우선순위가 저 줌레벨에서 이렇게 높을거라고 생각하시는지요?

<img src="https://github.com/pil0706/pil0706.github.io/blob/master/screenshots/positionofpois/japanese_embassy.png?raw=true">

저는 지도가 정치적인 논란거리로 사용되는것을 좋아하지 않습니다.
<br>
<br>
<br>
<br>
<br>
PS2 : Copenhagen 까꿍<br>
<br>
저는 구글이 어떤 도구를 사용하고 어떻게 만드는지 정말 진짜 알고싶습니다.<br>

<img src="https://github.com/pil0706/pil0706.github.io/blob/master/screenshots/positionofpois/copenhagen_pikabu.png?raw=true">

덴마크가 없어지자 마자, 코펜하겐이 나타납니다.<br>
까.....꿍!!!!!
<br>
<br>