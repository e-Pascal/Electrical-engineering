# Части 1. Пример выполнения и оформления
Расчёт линейного стабилизатора
Выполнил: Зероту В.Т.
Вариант 30
Задание 1
Таблица 1 – Параметры для подбора линейного стабилизатора 
№ИВ	Uвх_min, В	Uвх_max, В	Uвых, В	Iвых, мА	Company
30	19	20	17	180	Analog Devices

1.1 Выбор стабилизатора
Для формирования фильтра не были заданы все параметры, заданные по варианту, для того чтобы поисковая система не ограничивала результаты поиска. Например, по заданию данного варианта, выходное напряжение 19-20В. Если указать данный параметр в фильтре, то поисковая система попытается найти компонент с конкретным заданным напряжением и, скорее всего, не найдёт. Потому что производитель в характеристиках компонента указывает ДОПУСТИМЫЙ диапазон входного напряжения, например 3,3-20В. При выборе компонента необходимо чтобы ваш диапазон входных напряжений укладывался в диапазон, приведённый в спецификации на компонент. При выборе компонентов зачастую удобнее пользоваться сайтами производителей, на которых применяются более удобные фильтры для подбора, но в рамках данного задания необходимо воспользоваться только разрешённым (в данном примере я воспользовался сайтом дистрибьютером mouser.com).
 
Рис.1 – Настройка фильтра для выбора стабилизатора
Выбран линейный стабилизатор ADP7102. На рисунке 2 представлено общее описание характеристик стабилизатора. Для уточнения характеристик можно воспользоваться таблицами, приведёнными в этой же спецификации. Выбранный стабилизатор удовлетворяет параметрам индивидуального задания:
Uвх_мин 3,3 В (Input voltage range: 3.3 V to 20 V)
Uвх_мах 20 В (Input voltage range: 3.3 V to 20 V)
Uвых 1.22-19.8 (Adjustable output from 1.22 V to VIN – VDO) С учётом того, что Low dropout voltage (VDO – падение напряжения на стабилизаторе): 200 mV at 300 mA load (VDO при токе нагрузки 300мА составляет 200мВ)
Iвых_мах = 300мА (Maximum output current: 300 mA)

 
Рис.2 – Описание выбранного стабилизатора из спецификации
1.2 Расчёт схемы
 
Рис.3 – Типовая схема подключения стабилизатора 
В данной схеме необходимо произвести расчёт делителя напряжения R1 и R2. В соответствии со спецификацией рекомендуется выбирать резистор менее 200кОм. Примем R2 равным 10кОм. Воспользовавшись формулой, приведённой в спецификации, вычислим R1.
Vout=1.22 (1+R_1/R_2 )
R_1=R_2 (Vout/(1.22)-1)=10к(17/(1.22)-1)=129кОм 


1.3 Расчёт с учётом стандартного ряда номиналов резисторов
Для подбора резистора из ряда E24 я воспользовался сайтом https://www.radiolibrary.ru/reference/resistorseries/e24.html
 и выбрал R1 и R2  130к и 10к соответственно.
Vout=1.22 (1+R_1/R_2 )=1.22(1+130к/10к)=17,08 В
Для моделирования схемы (не обязательно) со стабилизатором от Analog Devices, можно воспользоваться программой LTspice.
 
Рис.4 – Проверка схемы в LTspice 
1.4 Схема
 
Рис.5 – Схема электрическая принципиальная 
1.5 Расчёт тока нагрузки
Iнагр=U_вых/R_нагр =(17 В)/(100 Ом)=0,17А=170мА
Не стоит путать ток, заданный по варианту и ток, рассчитанный в данном пункте. В варианте указан максимальный ток, который должен обеспечивать стабилизатор, но это совсем не значит, что ток, потребляемый нагрузкой, будет равен заданному в варианте. В задании для примера задано значение резистора, имитирующего нагрузку, 100 Ом.
1.6 Расчёт рассеивающей мощности
В данном задании необходимо использовать ток Iвых, заданный в варианте задания. Данный расчёт показывает какую мощность будет рассеивать стабилизатор при худших условиях работы (максимальном входном напряжении и максимальном заданным выходным током).
Pрасс=Iвых*(U_(вх_мах )- U_вых )=0.18 А*(20 В-17 В)=0,54 Вт
С учётом теплового сопротивления стабилизатора, можно рассчитать, насколько нагреется микросхема, при вычисленной мощности.
 
Рис.6 – Параметры теплового сопротивления
	Например, стабилизатор выбран в корпусе SOIC-8. Из таблицы используем параметр, который характеризует тепловое сопротивление микросхемы без учёта дополнительных радиаторов θJA = 48.5. Следовательно при заданной мощности нагрев микросхемы составит t= Pрасс* θJA=26.19 C°. При комнатной температуре 24 C° температура нагруженного стабилизатора составит приблизительно 60 C°. Расчёт приблизительный. Для уменьшения температуры стабилизатора при разработке топологии печатной платы прибегают к использованию дополнительных радиаторов в виде отдельных конструкций или выполняют прямо на плате в виде увеличенной площади металлизации.
С учётом вычисленной температуры и таблицы из спецификации, можно сделать вывод о том, что данный стабилизатор будет сохранять работоспособность в нагруженном состоянии.
 
Рис.7 – Абсолютные предельные значения рабочих параметров
