## Итоговая проверочная работа.

#### Этапы выполнения задания:

1. Создать репозиторий на GitHub
2. Нарисовать блок-схему алгоритма
3. Снабдить репозиторий оформленным текстовым описанием решения (файл README.md)
4. Написать программу, решающую поставленную задачу
5. Использовать контроль версий в работе над этим небольшим проектом (не должно быть так, что все залито одним коммитом, как минимум этапы 2, 3 и 4 должны быть расположены в разных коммитах)

### Задача:

Написать программу, которая из имеющегося массива строк формирует массив из строк, длина которых меньше либо равна 3 символа. Первоначальный массив можно ввести с клавиатуры, либо задать на старте выполнения алгоритма. При решение не рекомендуется пользоваться коллекциями, лучше обойтись исключительно массивами.

Примеры:

* ["hello", "2", "world", ":-)"] -> ["2", ":-)"]
* ["1234", "1567", "-2", "computer science"] -> ["-2"]
* ["Russia", "Denmark", "Kazan"] -> []

### Выполнение этапов:

1. Репозиторий на GitHub создан.

2. Блок-схема вложена в файле *_Flowchart.._*.

3. Файл *_README.md_* и файл *_.gitignore_* - созданы.

4. Программа, решающая поставленную задачу, вложена в файле *_Programs_*.

5. Выполнение работ производилось в несколько этапов и расположено в разных коммитах - минимум 6.

### Алгоритм решения:

Задаётся два массива: входящий, который задаётся с клавиатуры, и исходящий такого же размера. 
Формирование исходящего массива производится при помощи метода. Основой метода является цикл соразмерный размеру массива, внутри которого производится проверка условия каждого элемента входящего массива. 
Если элемент массива состоит из 3 или менее символов, элемент входящего массива заносится в count элемент исходящего массива. После создания первого элемнта, переменная *_count_* увеличивается на 1 и возвращается к циклу for в котором i также увеличивается на 1. И так проверяется весь входящий массив до конца.
Так как в исходный данных элементы массива указаны в ковычках, в цикле метода исключаются 2 знака, им соответствующие.

Вывод на печать входящего массива также производится с использованием метода. Метод учитывает использование запятой для разделения элементов. Последний элемент печатается без запятой.

Так как примера в данной задаче три и ввод данных производится с клавиатуры, условия уже внесены и расположены под неактивными разделами *_Пример..._*. Одновременно в расчёте может использоваться не более одного условия задачи. В условиях задачи предусмотрено отображение данных в кавычках и с разделеним запятой, за исключением последнего элемента.
 
Вывод на печать исходящего массива производится без использования выше указанного метода, так как размер исходящего массива меньше входящего. Используется обычный способ вывода, с использованием цикла и проверки массива на отсутствие пустых строк. Для корректного отображения запятых применён счётчик *_count_*, для учёта заполненных строк. В дальнейшем он вычитается из величины размера массива с целью корректного отображения последней запятой.


