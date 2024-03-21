# search_engine
 
Программа для нахождения наиболее релевантных файлов.

Для того чтобы программа работала корректно, необходимы 2 файла (config,requests) которые находятся в папке json.
Так же они должны быть заполнены по нормативу.

Папка json имеет 3 файла.

Как открыть и заполнить данные в json.
(нажимаете правой кнопкой мыши по файлу, выбираете "Открыть с помощью" и потом выбираете "Блокнот")

1. answers - В него записываются результаты работы поискового движка.

2. config - В нем вы указываете max_responses, максимальное количество вариантов в ответе.
А так же путь к файлу или файлам, в которых будет произведён поиск слов.
("../resources/Имя файла" пример "../resources/file001.txt").

3. requests - Он содержит запросы, которые необходимо обработать поисковому движку.

Пример:

    "requests": [

       "moscow is the capital of russia",
       "sit veniam",
       "good man elit"

    ]

В папку resources вы переносите файлы, которые необходимо обработать поисковому движку.
На дынный момент только txt формат.

После ввода данных во всех файлах запустите программу, нажав на project.
После завершения результат будет в папке answer и откройте answers.

// Для разрабочиков.

Среда разработки использовалась CLine.

Используется CMake VERSION 3.27 и C++ 23 VERSION.

Используется сторонние библиотеки: 

"nlohmann/json.hpp"

"gtest/gtest.h"
