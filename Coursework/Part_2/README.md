# Часть 2. Расчёт импульсного стабилизатора
Задание 1. Импульсный стабилизатор с регулируемым выходом
1.1 Выбрать импульсный стабилизатор напряжения с регулируемым выходным напряжением, удовлетворяющий параметрам, приведённым в таблице 2.1.
Таблица 2.1 – Параметры для подбора импульсного стабилизатора 
№ИВ	UВХ_MIN, В	UВХ_MAX, В	UВЫХ, В	IВЫХ, мА
1	5	6	3.5	160
2	5.5	7	3.5	200
3	6	7	3.5	300
4	6.5	8	3.5	300
5	7	10	4	350
6	7.5	9	4	300
7	8	11	4	230
8	8.5	13	5	200
9	9	14	5	300
10	9.5	12	5	300
11	10	11	5	200
12	10.5	11	5	220
13	11	13	6	300
14	10	11	5	220
15	11.5	12	6	300
16	12	15	6	400
17	12.5	15	6	300
18	13	15	7	250
19	13.5	14	7	300
20	14	16	7	300
21	14.5	17	8	170
22	15	18	8	300
23	15.5	17	9	300
24	16	18	9	270
25	16.5	17	10	300
26	17	18	11	180
27	17.5	19	12	200
28	18	20	12	230
29	18.5	20	13	250
30	19	20	11	400

П р и м е ч а н и е
№ИВ – номер индивидуального варианта
Uвх_min – входное минимальное напряжение
Uвх_max – входное максимальное напряжение
Uвых – номинальное выходное напряжение
Iвых – выходной ток
1.2 Рассчитать схему для стабилизатора в соответствии со спецификацией на выбранный компонент. Расчёт схемы включает в себя расчёт номиналов резисторов, конденсаторов и прочих пассивных компонентов, если они требуются в схеме. После вычисления точных значений номиналов подобрать ближайшие из ряда E24. 
1.3 Зарисовать итоговую схему с учётом номиналов, выбранных на этапе 1.2.  
1.4 Рассчитать ток Iнагр, который будет выдан стабилизатором в нагрузку при Rнагр  = 10 Ом.
1.5 Сделать вывод о том, выдержит ли стабилизатор нагрузку, эквивалентную Rнагр  = 10 Ом (если Iнагр < Iмах_стаб то стабилизатор выдержит данную нагрузку). Значение Iмах_стаб приведено в спецификации.
Задание 2. Импульсный стабилизатор с фиксированным выходом
2.1 Выбрать импульсный стабилизатор напряжения с фиксированным выходным напряжением, удовлетворяющий параметрам, приведёнными в табл. 2.2.
Таблица 2.2 – Параметры для подбора импульсного стабилизатора 
№ИВ	Uвх_min, В	Uвх_max, В	Uвых, В	Rнагр, Ом
1	14.5	18	5	8
2	15	17	3.3	15
3	15.5	16	5	10
4	8.5	11	3.3	6
5	9	11	5	8
6	9.5	13	3.3	7
7	10	14	5	20
8	10.5	12	3.3	13
9	11	12	5	15
10	11.5	13	3.3	14
11	12	13	5	10
12	12.5	14	3.3	8
13	13	15	5	9
14	13	14	5	10
15	13.5	15	3.3	16
16	14	15	5	12
17	14.5	16	3.3	8
18	15	16	5	16
19	15.5	17	3.3	22
20	16	18	5	12
21	16.5	17	3.3	11
22	17	18	5	8
23	17.5	20	3.3	11
24	18	20	5	9
25	18.5	20	3.3	13
26	19	22	5	18
27	12.5	20	3.3	9
28	13	20	5	5
29	13.5	18	3.3	12
30	14	18	5	10
П р и м е ч а н и е
№ИВ – номер индивидуального варианта
Uвх_min – входное минимальное напряжение
Uвх_max – входное максимальное напряжение
Uвых – номинальное выходное напряжение
Iвых – выходной ток
2.2 Рассчитать схему для стабилизатора в соответствии со спецификацией на выбранный компонент. Расчёт схемы включает в себя расчёт номиналов резисторов, конденсаторов и прочих пассивных компонентов, если они требуются в схеме (подобрать ближайшие значения из стандартного ряда E24). В случае, если в спецификации приведена схема и расчёты не требуются, указать в данном пункте «Схема приведена в спецификации».
2.3 Зарисовать итоговую схему.
2.4 Сделать вывод о том, выдержит ли стабилизатор нагрузку, эквивалентную Rнагр  = 10 Ом (если Iнагр < Iмах_стаб то стабилизатор выдержит данную нагрузку). Значение Iмах_стаб приведено в спецификации.
Требования к отчёту
	отчёт должен быть выполнен в электронном виде;
	отчёт должен содержать фрагменты фильтров с сайтов дистрибьютеров;
	отчёт должен содержать фрагменты схем из спецификации;
	отчёт должен содержать фрагменты таблицы из спецификации;
	отчёт должен содержать фрагменты формул из спецификации;
	рисунки в отчёте должны быть названы и пронумерованы;
	в случае, если схемы нарисованы от руки, к отчёту следует приложить фотографию схемы, если оформлены в Altium Designer – приложить скрин.
Загрузка отчёта 
Отчёт по части 2 выполняется в том же документе, что и часть 1 – является его продолжением, после чего должен быть прикреплён в системе ОРИОКС в разделе «Домашние задания»:
Дисциплина – Электротехника
Контрольное мероприятие – КР. Часть 2
Название задания – «Расчёт импульсных стабилизаторов напряжения»
Тип работы – Домашняя работа
Вариант – (указать номер варианта из таблицы)
Описание – (указать через запятую названия выбранных стабилизаторов)