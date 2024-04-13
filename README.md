# Домашнее задание №13 - Сравнение массивов (1 балл)

## Определения

_-1|0|1-сравнение_ - стандартный способ выражения операции одновременного сравнения на меньше,
равно и больше двух элементов. Стандарт следующий:
* Операция возвращает число меньше нуля, если первый аргумент меньше второго
* Операция возвращает ноль, если аргументы равны
* Операция возвращает число больше нуля, если первый аргумент больше второго

_Лексикографический порядок_ - стандартный способ сортировки последовательностей элементов, в
котором одна последовательность меньше второй, если первый элемент, отличающийся в ней от
соответствующего элемента второй последовательности, меньше него, либо если первая
последовательность заканчивается раньше второй. Известный пример - сортировка слов в словаре, где
слова - последовательности символов.

Примеры:
* аркада < армада
* арка < аркада

## Условие

Прочитать с клавиатуры два числа `N` и `M` типа `size_t`. Затем прочитать `N` чисел и сохранить их
в VLA-массив `A1` длины `N` в автоматической памяти. Затем прочитать `M` чисел и сохранить их в 
VLA-массив `A2` длины `M` в автоматической памяти.

Вывести результат операции -1|0|1-сравнения массивов `A1` и `A2` в лексикографическом порядке. Для
стабильности результатов и упрощения автоматической проверки решения выводить нужно не
произвольные числа меньше и больше нуля, а строго -1 или 1.

Программа должна работать корректно с массивами длины 0. Два массива длины 0 равны. Любой массив
ненулевой длины больше массива длины 0. Учтите, что создание VLA-массивов длины 0 запрещено
санитайзерами, используемыми при проверке решений.

Если какое-либо из чисел `N` и `M` больше 1000, нужно вывести сообщение об ошибке `Incorrect input`
и прервать выполнение программы.

## Пример №1

### Входные данные

```
5 4
0 1 2 3 4
0 1 2 4
```

### Выходные данные

```
-1

```

## Пример №2

### Входные данные

```
4 3
0 1 2 0
0 1 2
```

### Выходные данные

```
1

```

## Пример №3

### Входные данные

```
3 3
0 1 2
0 1 2
```

### Выходные данные

```
0

```
