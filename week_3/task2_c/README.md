# Задание 2
c: Напишите программу, реализующую алгоритм определения простых чисел (решето Эратосфена).
***
**Описание**:
***
Вводится число n. Если n<2, программа выводит сообщение об ошибке.
***
Если n корректен, вызывается метод findPrimes(int n) из класса SieveofEratosthenes, который выполняет следующие шаги:
***
1. Создаётся массив isPrime длиной n+1 и заполняется значениями true, предполагая, что все числа изначально простые.
2. Устанавливются значения для 0 и 1 как false, так как они не являются простыми числами.
3. Запускается цикл для алгоритма решета Эратосфена, начиная с 2, и помечает все кратные простых чисел как составные,
   устанавливая соответствующие индексы в массиве isPrime в false.
***
После завершения работы алгоритма выводятся все числа, которые помечены как простые (т.е. значения true в массиве isPrime), в диапазоне от 2 до n.