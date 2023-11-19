# Лекция №11. Общие свойства четырехполюсников
Электротехническое устройство, служащее для передачи энергии (сигналов) и имеющие по два входных и выходных зажима, называется `четырехполюсником`.  
Если внутри четырехполюсника нет источников энергии или они взаимно компенсируют друг друга, то такой четырехполюсник называют `пассивным` (рис. 8-1: а - идеальный трансформатор; б - частотный фильтр; в - мостовая схема).

<p align="center" > <img src="./pic/p2.png"></p>
<p align="center" >Рисунок 8 - 1</p> 

Рассмотрим свойства четырехполюсников в установившемся режиме при периодических синусоидальных токах и напряжениях. Это позволит в дальнейшем применить полученные результаты для анализа цепей при других формах сигналов.  

Для анализа свойств четырехполюсника установим зависимость между входным напряжением $\dot{U}_1$ и токами

$\dot{I}_1$ и входными
$\dot{U}_2$ и
$\dot{I}_2$ (рис. 8-2, где П - пассивная схема).

 
<p align="center" > <img src="./pic/p3.png"></p>
<p align="center" >Рисунок 8 - 2</p>

При выборе направлений напряжений и токов, указанных на рисунке, энергия передается от входа (клемма a-b) к сопротивлению нагрузки $Z_H$
  (клеммы c-d).  
Составим уравнение цепи методом контурных токов. В первый контур включим входные зажимы, во второй контур включим сопротивление нагрузки $\overline{Z}_H$.

```math
\overline{Z}_H \dot{I}_1 + \overline{Z}_{12} \dot{I}_2 + \overline{Z}_{13} \dot{I}_3 + ... + \overline{Z}_{1n} \dot{I}_n = \dot{U}_1
```
```math
\overline{Z}_{21} \dot{I}_1 + \overline{Z}_{22} \dot{I}_2 + \overline{Z}_{23} \dot{I}_3 + ... + \overline{Z}_{2n} \dot{I}_n = 0
```
```math
\overline{Z}_{n1} \dot{I}_1 + \overline{Z}_{n2} \dot{I}_2 + \overline{Z}_{n3} \dot{I}_3 + ... + \overline{Z}_{nn} \dot{I}_n = 0.  
```


Обозначим  $\overline{Z}_2{}_2$ = $\overline{Z'}_1{}_2$ + $\overline{Z}_H$,
где  $\overline{Z}_2{}_2$ - часть сопротивления второго контура, входящая в состав четырехполюсника.  
Учитывая, что $\dot{I}_2$ $\overline{Z}_H$ = $\dot{U}_2$:  
```math
\overline{Z}_{11} \dot{I}_1 + \overline{Z}_{12} \dot{I}_2 + ... + \overline{Z}_{1n} \dot{I}_n = \dot{U}_1
```
```math
\overline{Z}_{21} \dot{I}_1 + \overline{Z}_{22} \dot{I}_2 + ... + \overline{Z}_{2n} \dot{I}_n = - \dot{U}_2
```
```math
\overline{Z}_{n1} \dot{I}_1 + \overline{Z}_{n2} \dot{I}_2 + ... + \overline{Z}_{nn} \dot{I}_n = 0.
```

Все остальные уравнения содержат в правой части нули, что соответствует пассивному четырехполюснику.  
Решение системы уравнений:  
```math
\dot{I}_1 = \frac{\Delta_{11}}{\Delta} \dot{U}_1 - \frac{\Delta_{21}}{\Delta} \dot{U}_2;
``` 
```math
\dot{I}_2 = \frac{\Delta_{12}}{\Delta} \dot{U}_1 - \frac{\Delta_{22}}{\Delta} \dot{U}_2;
```  
Отношения  $\frac{\Delta_{11}}{\Delta}$,  $\frac{\Delta_{12}}{\Delta}$ имеют размерность проводимости.  
Обозначим  
```math
\frac{\Delta_{11}}{\Delta} = \overline{Y}_{11}; \frac{\Delta_{12}}{\Delta} = \overline{Y}_{21}; -\frac{\Delta_{22}}{\Delta} = \overline{Y}_{22}; -\frac{\Delta_{21}}{\Delta} = \overline{Y}_{12}.
```  
тогда уравнения четырехполюсника принимают вид:  
```math
\dot{I}_1 = \overline{Y}_{11} \dot{U}_1 + \overline{Y}_{12} \dot{U}_2;
```
```math
\dot{I}_2 = \overline{Y}_{21} \dot{U}_1 + \overline{Y}_{22} \dot{U}_2.
```    
 
В матричной форме:  
```math
\begin{bmatrix}
\overline{Y}_{11} & \overline{Y}_{12}\\
\overline{Y}_{21} & \overline{Y}_{22}
\end{bmatrix}.
\begin{bmatrix}
\dot{U}_1\\
\dot{U}_2
\end{bmatrix} =
\begin{bmatrix}
\dot{I}_1\\
\dot{I}_2
\end{bmatrix},
``` 
или  
 $\mathbf{\overline{Y} \dot{U} = \dot{I}}$.  
Для линейных уравнений, соответствующих линейным цепям $\Delta_{12} = \Delta_{21}$
 , поэтому  $Y_{12} = - Y_{21}$.  
Указанные коэффициенты называются Y-параметрами, а матрица Y-матрицей четырехполюсника. Как видно из записи уравнений четырехполюсников в Y-параметрах с учетом уравнения  $Y_{12} = - Y_{21}$
, пассивный четырехполюсник характеризуется тремя независимыми параметрами. Физический смысл Y-параметров можно определить по режимам короткого замыкания на выходе $(U_2 = 0)$
  и на входе $(U_1 = 0)$.
```math
Y_{11} = (\frac{\dot{I}_1}{\dot{U}_1})_{\dot{U}_2 = 0} - \text{входная проводимость при коротком замыкании на выходе}.  
```  
```math
Y_{12} = (\frac{I_1}{U_2})_{\dot{U}_1 = 0} - \text{передаточная (взаимная) проводимость при коротком замыкании на входе}.  
```  
```math
Y_{21} = (\frac{I_2}{U_1})_{\dot{U}_2 = 0} - \text{передаточная проводимость при коротком замыкании на выходе}.
```  
```math
Y_{22} = (\frac{I_2}{U_2})_{U_1 = 0} - \text{выходная проводимость при коротком замыкании на входе}.
```  
Решим систему уравнений относительно напряжений:  
 ```math
\mathbf{\dot{U} = \overline{Y}^{-1} \dot{I} = \overline{Z} \dot{I}},
```
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
