# Файл robots.txt - запрет индексации файлов и папок

Как закрыть доступ поисковым ботам к тем разделам сайта, которые не следует индексировать?

Проще всего это можно сделать с помощью файла **robots.txt**, который необходимо разместить в _корне сервера_ с кодировкой **ASCII**.

В этот файл можно внести несколько параметров.

Первый из них, это **User-agent**, который указывает на то, какому именно поисковику Вы хотите запретить индексацию тех или иных каталогов или страниц.

Вот самые распространённые в Рунете поисковые боты.

- **Рамблер:** StackRambler
- **Яндекс:** Yandex
- **Google:** Googlebot
- **MSN:** msnbot

Если Вы хотите отнести ваш запрет одновременно ко всем поисковым ботам, то поставьте вместо названия бота звездочку (\*).

Далее идет параметр **Disallow**, который указывает какие именно папки и файлы не нужно индексировать.

Например, нам необходимо запретить доступ к папкам с изображениями, скриптами, временными файлами, а также к файлам страниц ошибок.

Вот как это будет выглядеть:

```robots.txt
User-agent: *
Disallow: /error404.php
Disallow: /error500.php
Disallow: /img/
Disallow: /cgi-bin/
Disallow: /temp/
```
