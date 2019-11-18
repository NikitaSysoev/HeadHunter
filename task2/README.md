# HeadHunter

Необходимо расставить небоскрёбы в городе размером 6х6 клеток, учитывая следующие ограничения:

1. Высота любого небоскрёба: 1 - 6 этажей.

2. Количество этажей у небоскрёба должно быть уникальным по строке и по столбцу.

3. За более высокими небоскрёбами не видны более низкие.

4. Количество видимых небоскрёбов для строки или столбца (0 - любое количество).


Рассмотрим одну строку с двумя ограничениями на количество видимых небоскрёбов.

6							1

Слева должно быть видно шесть зданий, а справа – только одно.

Более высокие здания блокируют видимость более низких, поэтому возможен единственный способ расстановки:

6	1	2	3	4	5	6	1

Входные данные
Ограничения по количеству видимых небоскрёбов заданы строкой, состоящей из 24 чисел, разделенных запятыми.

Ограничения расположены по часовой стрелке.

Каждое число на рисунке обозначает порядковый номер числа-ограничения в строке.

0	1	2	3	4	5	
23							6
22							7
21							8
20							9
19							10
18							11
17	16	15	14	13	12	

Выходные данные
36 чисел, разделенные запятой.

Первые 6 - высоты небоскребов в верхней строке карты, вторые 6 чисел - высоты небоскребов во второй строке карты и т.д.


Примечания
Задача имеет единственное решение.

Напоминаем, что 0 в строке ограничений означает отсутствие ограничений.


Пример
2	2		
3							
6
4							3
4							
4		
2	2		
5	6	1	4	3	2	
4	1	3	2	6	5	
3	2	3	6	1	5	4	
6	5	4	3	2	1	6
4	1	2	5	6	4	3	3
4	3	4	2	5	1	6	
4		

Входные данные: 0,0,0,2,2,0,0,0,0,6,3,0,0,4,0,0,0,0,4,4,0,3,0,0

Выходные данные: 5,6,1,4,3,2,4,1,3,2,6,5,2,3,6,1,5,4,6,5,4,3,2,1,1,2,5,6,4,3,3,4,2,5,1,6