# Лекция №11. Общие свойства четырехполюсников
Электротехническое устройство, служащее для передачи энергии (сигналов) и имеющие по два входных и выходных зажима, называется `четырехполюсником`.  
Если внутри четырехполюсника нет источников энергии или они взаимно компенсируют друг друга, то такой четырехполюсник называют `пассивным` (рис. 8-1: а - идеальный трансформатор; б - частотный фильтр; в - мостовая схема).

<p align="center" > <img src="./pic/p2.png"></p>
<p align="center" >Рисунок 8 - 1</p> 
Рассмотрим свойства четырехполюсников в установившемся режиме при периодических синусоидальных токах и напряжениях. Это позволит в дальнейшем применить полученные результаты для анализа цепей при других формах сигналов.  

Для анализа свойств четырехполюсника установим зависимость между входным напряжением ![image](https://github.com/e-Pascal/Electrical-engineering/assets/149309758/b4947a9e-6005-4cb5-ac3c-936307da9084) и токами
![image](https://github.com/e-Pascal/Electrical-engineering/assets/149309758/a6d5e522-008c-4419-843a-abe78a600886) и входными
![image](https://github.com/e-Pascal/Electrical-engineering/assets/149309758/43e604a6-00df-4e79-a009-9afe18aadb17) и
![image](https://github.com/e-Pascal/Electrical-engineering/assets/149309758/4153664d-c12e-402a-b46e-d11d97219514) (рис. 8-2, где П - пассивная схема).

 
<p align="center" > <img src="./pic/p3.png"></p>
<p align="center" >Рисунок 8 - 2</p>

При выборе направлений напряжений и токов, указанных на рисунке, энергия передается от входа (клемма a-b) к сопротивлению нагрузки ![image](https://github.com/e-Pascal/Electrical-engineering/assets/149309758/ff80f8d1-59c0-4787-a1cb-6e9dc965cb8d)
  (клеммы c-d).  
Составим уравнение цепи методом контурных токов. В первый контур включим входные зажимы, во второй контур включим сопротивление нагрузки  
![image](https://github.com/e-Pascal/Electrical-engineering/assets/149309758/91607b4a-0b3b-4d04-aeae-904894d1cd80).
![image](https://github.com/e-Pascal/Electrical-engineering/assets/149309758/c41650ca-5ac3-4b71-9af0-3e497bb34a27)  
![image](https://github.com/e-Pascal/Electrical-engineering/assets/149309758/7d08f0cc-e0b0-4643-b7d9-72b8e85c06d2)  
![image](https://github.com/e-Pascal/Electrical-engineering/assets/149309758/3a225eca-3e99-480f-adf8-e18704c687d3).  
Обозначим  ![image](https://github.com/e-Pascal/Electrical-engineering/assets/149309758/ce909eb6-2f14-4e1e-8307-1ab875ab5fa2),
где  ![image](https://github.com/e-Pascal/Electrical-engineering/assets/149309758/a34fe13b-4920-4d5a-b121-94ec470f039a) - часть сопротивления второго контура, входящая в состав четырехполюсника.  
Учитывая, что  ![image](https://github.com/e-Pascal/Electrical-engineering/assets/149309758/2371a0c5-a576-441b-9ff6-28f439302f87):  
 ![image](https://github.com/e-Pascal/Electrical-engineering/assets/149309758/af7893b7-8847-4a50-8f7e-fe7c71c4ce6a)  
![image](https://github.com/e-Pascal/Electrical-engineering/assets/149309758/3d281044-cb63-459f-9a86-3bba7bea830f)  
![image](https://github.com/e-Pascal/Electrical-engineering/assets/149309758/f38e5078-fb15-48a1-a3c1-4a33fb8ea7fa).  

Все остальные уравнения содержат в правой части нули, что соответствует пассивному четырехполюснику.  
Решение системы уравнений:  
 ![image](https://github.com/e-Pascal/Electrical-engineering/assets/149309758/f0731544-3fa3-4780-b286-d82a454c0e74);  
 ![image](https://github.com/e-Pascal/Electrical-engineering/assets/149309758/59a6f0c8-8192-49d5-b065-2874bfddec96).  
Отношения  ![image](https://github.com/e-Pascal/Electrical-engineering/assets/149309758/f421f215-2a84-42ec-a930-20ce770b1419)
,  ![image](https://github.com/e-Pascal/Electrical-engineering/assets/149309758/1046ee61-57ab-410d-8746-9f516f8d7169)
 имеют размерность проводимости.  
Обозначим  
![image](https://github.com/e-Pascal/Electrical-engineering/assets/149309758/b6d9d30e-e93c-4546-9fba-0158531dd9eb);  
![image](https://github.com/e-Pascal/Electrical-engineering/assets/149309758/f90b6646-d84d-4cb3-9411-7417706b44e9);  
![image](https://github.com/e-Pascal/Electrical-engineering/assets/149309758/2fb45f37-9f27-4de4-ad20-92f5f4220dba);  
![image](https://github.com/e-Pascal/Electrical-engineering/assets/149309758/850f12d9-1244-45fd-8eb8-0baa7c0874f2),  
тогда уравнения четырехполюсника принимают вид:  
![image](https://github.com/e-Pascal/Electrical-engineering/assets/149309758/7e1bfd1b-d830-4ab8-9685-4ed8e5c983f1);  
![image](https://github.com/e-Pascal/Electrical-engineering/assets/149309758/7fbf9a58-45ed-4125-a55b-d8322162b1aa).  
В матричной форме:  
 ![image](https://github.com/e-Pascal/Electrical-engineering/assets/149309758/5e6de1b2-e293-4c9e-b43c-4a83f3baecf4),  
или  
 ![image](https://github.com/e-Pascal/Electrical-engineering/assets/149309758/5418795e-1973-4448-979a-eae4df6108db).  
Для линейных уравнений, соответствующих линейным цепям ![image](https://github.com/e-Pascal/Electrical-engineering/assets/149309758/1639616f-9b14-405a-991d-d1c4e70a5fb2)
 , поэтому  ![image](https://github.com/e-Pascal/Electrical-engineering/assets/149309758/6f40d31d-98ec-450b-8a1a-2fabd779c827).  
Указанные коэффициенты называются Y-параметрами, а матрица Y-матрицей четырехполюсника. Как видно из записи уравнений четырехполюсников в Y-параметрах с учетом уравнения  ![image](https://github.com/e-Pascal/Electrical-engineering/assets/149309758/a4044079-af92-4710-b674-e0fb62d923d9)
, пассивный четырехполюсник характеризуется тремя независимыми параметрами. Физический смысл Y-параметров можно определить по режимам короткого замыкания на выходе ![image](https://github.com/e-Pascal/Electrical-engineering/assets/149309758/b969e604-7779-4155-ba13-db5d74462085)
  и на входе ![image](https://github.com/e-Pascal/Electrical-engineering/assets/149309758/f1d9b3b0-4c1e-4c25-82ba-5502f6aef785).  
![image](https://github.com/e-Pascal/Electrical-engineering/assets/149309758/43ca8062-dcce-452d-be52-4bd33a78d7fb) - входная проводимость при коротком замыкании на выходе.  
![image](https://github.com/e-Pascal/Electrical-engineering/assets/149309758/ca877ba7-53a3-4860-9eff-1b76fb12404c) - передаточная (взаимная) проводимость при коротком замыкании на входе.  
![image](https://github.com/e-Pascal/Electrical-engineering/assets/149309758/8e6e7eff-40d9-4205-a416-21906fe3a641) - передаточная проводимость при коротком замыкании на выходе.  
![image](https://github.com/e-Pascal/Electrical-engineering/assets/149309758/4d8758b1-4fec-4a2c-ada5-f89fac314487) - выходная проводимость при коротком замыкании на входе.  
Решим систему уравнений относительно напряжений:  
 ![image](https://github.com/e-Pascal/Electrical-engineering/assets/149309758/3e0bd241-fd8c-4d1c-aa14-7374e323df49),  
где ![image](https://github.com/e-Pascal/Electrical-engineering/assets/149309758/5f3445ba-9f0a-493f-bda4-88407bddeeb5)  
Или в развернутом виде  
![image](https://github.com/e-Pascal/Electrical-engineering/assets/149309758/d216d560-f275-4343-b065-2ee1c63c32f8)  
![image](https://github.com/e-Pascal/Electrical-engineering/assets/149309758/375b5f4e-4707-4ba5-8199-c5e1c28c577b)

 
Два из четырех параметров связаны между собой:  
 ![image](https://github.com/e-Pascal/Electrical-engineering/assets/149309758/3c0b46d4-c561-48e3-9c78-4f263069fa48)  

Физический смысл Z-параметров четырехполюсника можно определить по режимам холостого хода на выходе ( ) и на входе ( ).
 ![image](https://github.com/e-Pascal/Electrical-engineering/assets/149309758/3ee37b3a-0840-4091-b926-e036d0663f9d) - входное сопротивление в режиме холостого хода на выходе.  
![image](https://github.com/e-Pascal/Electrical-engineering/assets/149309758/658f3ee6-a4c0-49dc-8bf6-9173df3044ea) - передаточное (взаимное) сопротивление в режиме холостого хода на входе.  
 ![image](https://github.com/e-Pascal/Electrical-engineering/assets/149309758/951bcdda-2998-40e9-adc8-497ec73c2ca1) - передаточное сопротивление в режиме холостого хода на выходе.  
 ![image](https://github.com/e-Pascal/Electrical-engineering/assets/149309758/289074a0-a33c-45b4-a2fd-fdd357c465d3) - выходное сопротивление зажимов 22’ в режиме холостого хода на входе.  
Во многих практических случаях удобно когда система уравнений решена относительно выходных напряжений и тока:  
 ![image](https://github.com/e-Pascal/Electrical-engineering/assets/149309758/a04f79d9-337b-4c48-8263-2250fa564dc1)  
![image](https://github.com/e-Pascal/Electrical-engineering/assets/149309758/338952c1-d2de-4f62-a9da-946012a299f6)  

 
Параметры A, B, C, D в общем случае комплексные. Их можно выразить, например, через Z-параметры.  
Решая второе уравнение Z-параметров относительно тока ![image](https://github.com/e-Pascal/Electrical-engineering/assets/149309758/06956e9a-1cf1-40e7-90d1-9e80c78c7c7f), получим:  
 ![image](https://github.com/e-Pascal/Electrical-engineering/assets/149309758/bf1277de-ecf8-48cc-9187-88dcb28bdd4b)  

Сопоставив со вторым уравнением в A-параметрах, получаем:  
 ![image](https://github.com/e-Pascal/Electrical-engineering/assets/149309758/7f8c3b44-36f7-48f7-8b85-849ab55742cb); ![image](https://github.com/e-Pascal/Electrical-engineering/assets/149309758/681057d5-4239-4947-ae96-23d3275d0eda)
  
 Подставим ![image](https://github.com/e-Pascal/Electrical-engineering/assets/149309758/32ab9b73-378e-4fc6-9c69-847ae2cb48ec) в первое уравнение в Z-параметрах:  
 ![image](https://github.com/e-Pascal/Electrical-engineering/assets/149309758/189949bd-35b8-41cf-a9fe-5c2d952181a1)  

Таким образом  
 ![image](https://github.com/e-Pascal/Electrical-engineering/assets/149309758/5c21d8ac-ad5d-41a5-bc86-1d3b2e919d83);  
 ![image](https://github.com/e-Pascal/Electrical-engineering/assets/149309758/0b0f5c1a-8e4a-4f73-92db-b5429d808f33)  

Нетрудно убедиться, что AD-BC=1.  
Физический смысл А-параметров:  
![image](https://github.com/e-Pascal/Electrical-engineering/assets/149309758/13343a5d-44ee-46a9-9ce5-1a1f6f8ff601) - передаточное отношение напряжений в режиме холостого хода на выходе.  
![image](https://github.com/e-Pascal/Electrical-engineering/assets/149309758/b5e22c60-f1a7-437c-8024-ff04840eebaf) - передаточное сопротивление при коротком замыкании на выходе.  
![image](https://github.com/e-Pascal/Electrical-engineering/assets/149309758/a2994182-77f8-469e-89a2-796a5922687c) - передаточная проводимость в режиме холостого хода на выходе.  
![image](https://github.com/e-Pascal/Electrical-engineering/assets/149309758/16ef4690-bbfc-4985-bb90-69fbbfde62ef) - передаточное отношение токов при коротком замыкании на выходе.  
При обратном питании с учетом изменения знаков токов получим:  
 ![image](https://github.com/e-Pascal/Electrical-engineering/assets/149309758/4e666acc-c8ce-4fbf-ab56-c7883ca2a302)  
При этом сохраняется соотношение
AD-BC=1  
Для формирования уравнений при смешанном соединении четырехполюсников применяются еще два уравнения в H-параметрах и G-параметрах:  
 ![image](https://github.com/e-Pascal/Electrical-engineering/assets/149309758/7794d67d-2fea-4349-a8e5-4b9675316b5f)  
![image](https://github.com/e-Pascal/Electrical-engineering/assets/149309758/3f4effed-b303-4a56-8a78-9cc85dc245d2)  
![image](https://github.com/e-Pascal/Electrical-engineering/assets/149309758/5975978a-5ca6-432a-bcf5-d34fc3fba652)  
![image](https://github.com/e-Pascal/Electrical-engineering/assets/149309758/4b34a056-a44b-4859-9e82-e736a71c9047)  

 
 
 
Физический смысл предлагаем установить читателю.
