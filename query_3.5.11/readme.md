# Задание

Проанализировать, в каком порядке и с каким интервалом пользователь отправлял последнее верно выполненное задание каждого урока. Учитывать только студентов, прошедших хотя бы один шаг из всех трех уроков. В базе занесены попытки студентов  для трех уроков курса, поэтому анализ проводить только для этих уроков.

Для студентов прошедших как минимум по одному шагу в каждом уроке, найти последний пройденный шаг каждого урока - крайний шаг, и указать:
имя студента;  
номер урока, состоящий из номера модуля и через точку позиции каждого урока в модуле;  
время отправки  - время подачи решения на проверку;  
разницу во времени отправки между текущим и предыдущим крайним шагом в днях, при этом для первого шага поставить прочерк ("-"), а количество дней округлить до целого в большую сторону.

Столбцы назвать  Студент, Урок,  Макс_время_отправки и Интервал  соответственно. Отсортировать результаты по имени студента в алфавитном порядке, а потом по возрастанию времени отправки.

# Реализация
выборка столбцов и их именование,  
табличные выражения,   
соединение таблиц,   
условие отбора,   
функции CONCAT(), IFNULL() и FROM_UNIXTIME(),   
оконные функции,   
условие отбора в запросах группировки,   
сортировка

## Фрагмент логической схемы базы данных
<img width="352" alt="изображение" src="https://github.com/NickKulibaba/Interactive_simulator_SQL/assets/115520387/96cc464e-8825-44cb-926e-056748c533cd">

## SQL-запрос
<img width="878" alt="изображение" src="https://github.com/NickKulibaba/Interactive_simulator_SQL/assets/115520387/a1d53928-f4f7-4f51-8f5b-67ec47e54e4f">

## Результат
<img width="434" alt="изображение" src="https://github.com/NickKulibaba/Interactive_simulator_SQL/assets/115520387/bacce6de-aaf4-4447-a90b-46f5535c9e50">.  
<img width="437" alt="изображение" src="https://github.com/NickKulibaba/Interactive_simulator_SQL/assets/115520387/b5580a0f-4aa5-4667-a9f6-2d398f0741d7">

