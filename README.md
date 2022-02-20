
Linux terminal (GitBash) commands




 1) Посмотреть где я 
- pwd
 2) Создать папку 
- mkdir papka 
 3) Зайти в папку 
- cd papka
 4) Создать 3 папки
 - mkdir papka1 papka2 papka3
 5) Зайти в любоую папку 
- cd papka1
 6) Создать 5 файлов (3 txt, 2 json) 
- touch text1.txt text2.txt text3.txt text1.json text2.json
 7) Создать 3 папки 
- mkdir papka{1..3}
 8) Вывести список содержимого папки 
- ls
 9) вывести расширенный список содержимого
 - ls -la
10)	вывести список содержимого по дате создания
 - ls -lt
11) вывести список по дате обращения к файлу 
- ls -lu
 12) Открыть любой txt файл 
- vim text.txt
 13) войти в режим редактирования
 - i
	написать что-нибудь (abirvalg)
 14) выйти из режима редактирования
 - esc
15) сохранить 
- :wq
16) сохранить под новым именем 
- :sav newtext.txt
17) сохранить и выйти 
- :wq
 18) Выйти из папки на уровень выше 
- cd ..
19) выйти на два уровня выше 
- cd ../..
20) переключиться на последнюю посещенную папку
 - cd -
21) переместить любые 2 файла, которые вы создали, в любую другую папку 
- mv text1.txt text2.txt papka1
22) скопировать любые 2 файла, которые вы создали, в любую другую папку 
- cp text3.txt text4.txt papka2
23) Найти файл по имени 
- find text.txt
24) просмотреть содержимое в реальном времени (команда grep)
 - tail -f text.txt | grep privet
25) выйти 
- ctrl+c
26) вывести несколько первых строк из текстового файла 
- head -3 text.txt
27) вывести несколько последних строк из текстового файла 
- tail -3 text.txt
28) просмотреть содержимое длинного файла (команда less)
 - less text.txt
29) выйти
 - q
30) вывести дату и время 
- date

=========

*
 1) Отправить http запрос на сервер.

- http://162.55.220.72:5005/terminal-hw-request 
	запрос: curl "http://162.55.220.72:5005/terminal-hw-request"
	ответ: {"Intro":"Hello!! This is your the first response from server","Tasks":{"Task_1":"Send the next URL in terminal: http://162.55.220.72:5005/get_method?name=(set_your_String)&age=(set_your_number)","result":["Your_String","Your_number"]}}
	выполняем: curl "http://162.55.220.72:5005/get_method?name=(Anastasia)&age=(25)"
	ответ: ["(Anastasia)","(25)"]

 2) Написать скрипт который выполнит автоматически пункты 3, 4, 5, 6, 7, 8, 13

vim script.sh

#!/bin/bash
mk
dir papka

cd papka

mkdir papka{1..3}

cd papka1

touch text1.txt text2.txt text3.txt text1.json text2.json

mkdir papka{1..3}

ls -la

mv text1.txt text2.txt papka1

esc

:wq

./script.sh

=========
