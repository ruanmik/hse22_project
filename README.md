# hse22_project

[Ссылка на колаб](https://colab.research.google.com/drive/1vYeFGDNIH_A2cvPpHHsZE7ao4qlSKj0v?usp=sharing)

#### Выбранные геномы

Вид |	Уровень сборки | GC%
---|---|---
Leishmania sp. Ghana 2012 LV757 |  Chromosome | 59,6694
Leishmania infantum JPCM5 |  Chromosome |  59,5663
Leishmania donovani |  Chromosome |  59,1146
Leishmania orientalis |  Chromosome |  59,7148
Leishmania martiniquensis |  Chromosome |  59,8521

#### Анализ аннотированных генов

Вид |	Длина генома |	Количество экзонов |	Длина покрытия экзонами |	Доля покрытия экзонами
---|---|---|---|---
Ghana |	35953538.0 |	8119.0 |	14915813.0 |	0.415
Infantum |	32122061.0 |	8241.0 |	15607169.0 |	0.486
Donovani |	32444968.0 |	8083.0 |	14824824.0 |	0.457
Orientalis |	34194276.0 |	8158.0 |	15803203.0 |	0.462
Martiniquensis |	32413670.0 |	7967.0 |	14791807.0 |	0.456


#### Предсказываем участки Z-DNA

Вид |	Количество предсказанных Z-DNA | 	Количество участков с ZH-score > 500 |	Общая длина участков с ZH-score > 500
---|---|---|---
Ghana |	295535.0 |	8503.0 |	91738.0
Infantum |	277951.0 |	9051.0 |	98310.0
Donovani |	283432.0 |	9151.0 |	99396.0
Orientalis |	347095.0 |	9141.0 |	97978.0
Martiniquensis |	241723.0 |	6741.0 |	72132.0

##### Гистограммы распределений ZH-score > 500

<img width="445" alt="image" src="https://user-images.githubusercontent.com/80822257/173908192-4df4478c-1a26-494d-81d8-a1a52906a476.png"><img width="445" alt="image" src="https://user-images.githubusercontent.com/80822257/173908236-91f96355-075b-49aa-bddc-9fd4d3f5bb47.png">
<img width="445" alt="image" src="https://user-images.githubusercontent.com/80822257/173908283-4327f3dd-895a-4e39-83d7-9964fdabc83c.png"><img width="445" alt="image" src="https://user-images.githubusercontent.com/80822257/173908320-82f28e37-e602-45ce-a97a-f02c02cf626a.png">
<img width="468" alt="image" src="https://user-images.githubusercontent.com/80822257/173908385-ad42056d-e37e-4a73-9597-cba6423d7ec7.png">

#### Ассоциируем предсказанные участки Z-DNA с промотерами генов

<img width="792" alt="image" src="https://user-images.githubusercontent.com/80822257/173909605-ca4d93f8-68f2-476e-ad3a-75fbc9b2f706.png">
<img width="923" alt="image" src="https://user-images.githubusercontent.com/80822257/173909650-90f9d48f-033f-4549-be33-4899832d1380.png">
<img width="923" alt="image" src="https://user-images.githubusercontent.com/80822257/173909689-a5dedcc4-4b2b-4fbf-83f5-e2e95198f5f9.png">
<img width="869" alt="image" src="https://user-images.githubusercontent.com/80822257/173909720-7be56f30-8657-4c91-8290-5d4e27d77875.png">
<img width="943" alt="image" src="https://user-images.githubusercontent.com/80822257/173909756-fb00fba5-1690-4e1b-b334-3fd737f497e9.png">

#### Кластеризация:

Заметим, что наибольшая группа по количеству геномов в кластере - 5 уникальных геномов, поэтому кластеры подбираем по ним

<img width="564" alt="image" src="https://user-images.githubusercontent.com/80822257/173918368-034aa1d2-2f4e-404d-be2e-ce05fe0d1d68.png">

Для каждого вида выделили 10 кластеров

Donovani |	Ghana |	Infantum |	Martiniquensis |	Orientalis
---|---|---|---|---
CBZ31141.1 |	KAG5512547.1 |	CAM65205.1 |	KAG5488124.1 |	KAG5488272.1
CBZ37188.1 |	KAG5494227.1 |	CAM71208.1 |	KAG5469315.1 |	KAG5468963.1
CBZ31101.1 |	KAG5512511.1 |	CAM65165.1 |	KAG5488087.1 |	KAG5488234.1
CBZ31143.1 |	KAG5512549.1 |	CAM65207.1 |	KAG5488126.1 |	KAG5488274.1
CBZ34238.1 |	KAG5504731.1 |	CAM68144.1 |	KAG5478632.1 |	KAG5478420.1
CBZ32864.1 |	KAG5509223.1 |	CAM66767.1 |	KAG5482825.1 |	KAG5483003.1
CBZ38514.1 |	KAG5489215.1 |	CAM72642.1 |	KAG5463899.1 |	KAG5464630.1
CBZ38495.1 |	KAG5489197.1 |	CAM72661.1 |	KAG5463880.1 |	KAG5464611.1
CBZ32718.1 |	KAG5509713.1 |	CAM66618.1 |	KAG5483314.1 |	KAG5483732.1
CBZ36030.1 |	KAG5497772.1 |	CAM69870.1 |	KAG5472224.1 |	KAG5472603.1

В папке alignments - приведены файлы с множественными белковыми выравниваниями

#### Визуализация расположения участков Z-DNA для каждого выбранного кластера

1 кластер

<img width="474" alt="image" src="https://user-images.githubusercontent.com/80822257/173918847-59685a12-1664-4945-aa22-b002927b1405.png"><img width="474" alt="image" src="https://user-images.githubusercontent.com/80822257/173918885-4ad281d0-fdaa-4476-b495-d71f0820c3f7.png"><img width="474" alt="image" src="https://user-images.githubusercontent.com/80822257/173918937-d431ffa7-bcc1-4333-8e11-9ebfb2007802.png">

2 кластер

<img width="474" alt="image" src="https://user-images.githubusercontent.com/80822257/173919206-df41063b-7bd6-43bc-8bda-a78ea77e2214.png"><img width="474" alt="image" src="https://user-images.githubusercontent.com/80822257/173919262-f625fbf4-fbee-4eb2-beb9-c67fcc65c79e.png">


3 кластер

<img width="474" alt="image" src="https://user-images.githubusercontent.com/80822257/173919480-0890f35d-ed2d-49cf-94c0-076cebfb6241.png"><img width="474" alt="image" src="https://user-images.githubusercontent.com/80822257/173919547-2b204a45-e014-457b-a270-fd98a7b4d81c.png">


4 кластер

<img width="474" alt="image" src="https://user-images.githubusercontent.com/80822257/173919637-57d518aa-6813-4de7-bf7d-4e3c23d933c5.png"><img width="474" alt="image" src="https://user-images.githubusercontent.com/80822257/173919670-56424521-70bd-45a4-94b9-b0f174cade21.png"><img width="474" alt="image" src="https://user-images.githubusercontent.com/80822257/173919730-1611699a-9c62-431e-8cd6-3ff1252a3005.png">


5 кластер

<img width="474" alt="image" src="https://user-images.githubusercontent.com/80822257/173919792-8243dbed-1905-49b1-823e-e588290c0526.png"><img width="474" alt="image" src="https://user-images.githubusercontent.com/80822257/173919850-80a2b6d9-bfe9-4cf2-bc79-6e7542f2c052.png">


6 кластер

<img width="474" alt="image" src="https://user-images.githubusercontent.com/80822257/173919917-824cc573-450b-460b-bfa1-fdd4819588d5.png"><img width="474" alt="image" src="https://user-images.githubusercontent.com/80822257/173919961-c414c03b-3390-4bee-bf22-016158a42111.png">


7 кластер

<img width="474" alt="image" src="https://user-images.githubusercontent.com/80822257/173920046-3b9b00e4-bbeb-427e-b77a-c1d5ddfa5168.png"><img width="474" alt="image" src="https://user-images.githubusercontent.com/80822257/173920091-835cb2d4-e72b-4d32-a739-168f51734a2b.png"><img width="474" alt="image" src="https://user-images.githubusercontent.com/80822257/173920155-8b3a98f2-cd84-4d16-a081-187d326863f5.png">


8 кластер

<img width="474" alt="image" src="https://user-images.githubusercontent.com/80822257/173920237-2f35e31e-1392-4db9-98a3-29196dd95423.png"><img width="474" alt="image" src="https://user-images.githubusercontent.com/80822257/173920279-f41195c0-ffdb-4daa-8833-bd4b41e1693c.png">


9 кластер

<img width="474" alt="image" src="https://user-images.githubusercontent.com/80822257/173920381-55dc7f56-8848-4803-a31d-b8d621900665.png"><img width="474" alt="image" src="https://user-images.githubusercontent.com/80822257/173920420-8367d4c5-0b5e-4213-a638-3ab1930e339e.png"><img width="474" alt="image" src="https://user-images.githubusercontent.com/80822257/173920447-556a7a87-0dbf-4898-b9d5-4988e1f0fef9.png">


10 кластер

<img width="474" alt="image" src="https://user-images.githubusercontent.com/80822257/173920515-992659eb-fa45-4139-a60e-c5486036245e.png"><img width="474" alt="image" src="https://user-images.githubusercontent.com/80822257/173920581-303f529e-1b3c-419b-b503-9a897412ad0f.png"><img width="474" alt="image" src="https://user-images.githubusercontent.com/80822257/173920633-9abbb223-9ed9-4e66-85aa-226da2fc71c8.png">
