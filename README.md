Данный проект реализован в качестве решения тестового задания на конкурс в собеседование в компанию "Гарда".

Проект реализует первые 10 пунктов технического задания и реализован на C++ с использованием дополнительных библиотек.

В корневой структуре проекта присутствуют файлы:

Client.cpp - это код для CLI-клиента Calculator Server.

Server.cpp - это код серверной части Calculator Server.

CmakeLists.txt - cmake-скрипт, который отвечает за сборку проекта

.clang-format - файл с кодестайлом, которому соответствует проект

Docker - файл конфигурации Docker, для запуска проекта

Папка include/, в которой хранятся подключаемые библиотеки

В программе используется библиотека cpp-httlib: https://github.com/yhirose/cpp-httplib.h

Это файл include/httlib.h. Эта библиотека используется для написания клиент-серверных приложений.

Так же в программе используется библиотека nlohmann::json для парсинга и передачи json-данных во время работы программы:https://github.com/nlohmann/json

Это файл include/json.hpp.

Библиотека check_correct.h написана мной, она содержит функцию, которая проверяет численное выражение на синтаксическую корректность

Библиотеки eval.h и calculator.h тоже написаны мной в ходе прохождения курса по C++ от Школы Анализа Данных Яндекс, с которой у нас совместная магистерская программа.

Она не использует в своей работе обратную польскую запись, а преобразует исходное выражение в AST (https://en.wikipedia.org/wiki/Abstract_syntax_tree) на основе математического аппарата формальной грамматики.
Подробее можете ознакомиться //фото


