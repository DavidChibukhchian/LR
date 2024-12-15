1. Чтобы собрать проект, нужно запустить скрипт build.sh в корневой папке проекта. Для запуска самой программы нужно использовать файл LR1, который появится в корневой папке проекта после сборки.

2. Грамматика задается в файле grammar.txt в корневой папке проекта. Если грамматика не LR1, то после запуска программы будет ошибка "bad grammar". После запуска программы нужно написать количество тестов, которые будет проверять LR1 автомат. Далее должны идти сами слова по одному на отдельной строке. На каждое слово будет дан ответ "YES" или "NO" в зависимости от того, принадлежит ли слово грамматике.

3. Проект предоставляет два способа считывания данных - из файла или из стандартного потока ввода, за это отвечают классы ConsoleReader и FileReader. Альтернативный способ ввода грамматики - через стандартный поток ввода - закомментирован в main.cpp.

4. Парсингом грамматики занимается класс Parser. Сама грамматика - класс Grammar. Внутри грамматики реализован алгоритм удаления непорождающих нетерминалов - это сделано для того, чтобы насчет массива FIRST в алгоритме LR1 был полностью корректен.
