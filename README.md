Access log parser
Задача
Имеется обычный http access_log файл. Требуется написать PHP скрипт, обрабатывающий этот лог и выдающий информацию о нём в json виде. Требуемые данные: количество хитов/просмотров, количество уникальных url, объем трафика, количество строк всего, количество запросов от поисковиков, коды ответов.

Пример запуска скрипта
#!/bin/bash

php parser.php --file=./acess.log

Результат
{ "views": 16, "urls": 5, "traffic": 212816, "crawlers": { "Google": 2, "Yandex": 0, "Bing": 0, "Baidu": 0 }, "status_codes": { "200": 14, "301": 2 } }