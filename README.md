<h1>Итоговая контрольная по основному блоку </h1>

<h2>Условие задачи : </h2>

<h3> 
Написать программу, которая из имеющегося массива строк формирует новый массив из строк, длина которых меньше, либо равна 3 символам. Первоначальный массив можно ввести с клавиатуры, либо задать на старте выполнения алгоритма. При решении не рекомендуется пользоваться коллекциями, лучше обойтись исключительно массивами.
</h3>

<h2>Основные этапы решения задачи : </h2>

<ol>
  <li>Функция вывода на печать элементов массива</li>
  <li>Функция создания массива из вводимых пользователем с клавиатуры значений</li>
  <li>Функция создания нового массива, с элементами по заданному в условии критерию</li>
</ol>

<h2>1. Функция вывода на печать элементов массива "PrintArray"</h2>
<h3>Создаём функцию типа void, принимающую на вход одномерный массив типа string. В теле функции цикл for со счётчиком. Цикл выполняется пока значение счётчика меньше  длинны массива (array.Length). В теле цикла - вывод в консоль элементов массива, по индексу счётчика, который при инициации цикла равен 0. Для разделения элементов, используется дополнительная функция консольного вывода символов ", "</h3>

<h2>2. Функция создания массива из вводимых пользователем с клавиатуры значений "Vvod"</h2>
<h3>Функция типа string, возвращает массив значений, вводимых пользователем с клавиатуры. В теле функции :
<ol><li>Вывод в консоль информационного сообщения пользователю "Введите значения череp запятую в одну строку : ". После чего пользователь вводит значения. По окончании ввода, нажимает клавишу Enter.</li>
<li>Создание переменной типа string, которой присвается ввод от пользователя функцией Console.ReadLine() </li>
<li> Строкове значение, полученное из ввода, преобразуем в массив, строковой функцией Split(). Разделитель значений для функции - ","</li>
<li>Возвращаем массив из введённых пользователем значений.</li>
</ol>

<h2>3. Функция создания нового массива, с элементами по заданному в условии критерию "Len3_array"</h2>
<h3> Условия по которому значения помещаются в новый массив - количество символов, меньше или равное 3. Создаём функцию, возвращающую массив типа string. В теле функции : </h3>
<ol>
<li> Получаем из функции "Vvod" массив значений и присваеваем его одномерному массиву типа string</li>
<li> Создаём переменную типа string без значения, для конкатенации к ней элементов по заданному условию </li>
<li> Создаём цикл for. Цикл инициируется с счётчиком типа int, начальное значение которого - 0. Условие цикла - значения счётчика меньше длинны массива. В конце цикла счётчик увеличивается на 1. В теле цикла проверяется длина значения. Если она меньше или равна 3, значение конкатенируется к переменной и добавляется символ ",", для последующего разбиения на массив функцией Split().  </li>
<li>После выхода из цикла от полученной строки значений, удаляется последний символ ","</li>
<li>Создаётся массив значений из строковой переменной с помощью функции Split(). Разделитель - символ ","</li>
<li>Массив возвращается из функции и передаётся в функцию "PrintArray" для вывода значений в консоль.</li>
</ol>
