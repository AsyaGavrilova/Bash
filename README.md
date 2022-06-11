# Домашнее задание № 1
1) Посмотреть где я
> pwd
2) Создать папку
> mkdir hw
3) Зайти в папку
> cd hw
4) Создать 3 папки
> mkdir a b c
5) Зайти в любоую папку
> cd a
6) Создать 5 файлов (3 txt, 2 json)
> touch f1.txt f2.txt f3.txt f4.json f5.json
7) Создать 3 папки
> mkdir a1 a2 a3
8) Вывести список содержимого папки
> ls -la
9) Открыть любой txt файл
> cat f1.txt
10) Написать туда что-нибудь, любой текст
> cat >> f1.txt 
11) Сохранить и выйти
> Enter, Ctrl + C
12) Выйти из папки на уровень выше
> cd ..
13) Переместить любые 2 файла, которые вы создали, в любую другую папку
> mv a/{f4.json,f5.json} b/  
14) Скопировать любые 2 файла, которые вы создали, в любую другую папку
> cp a/{f1.txt,f2.txt} c/
15) Найти файл по имени
> find . -name "f1.txt"
16) Просмотреть содержимое в реальном времени (команда grep) изучите как она работает
> tail -f a/f1.txt
17) Вывести несколько первых строк из текстового файла
> head -3 f1.txt
18) Вывести несколько последних строк из текстового файла
> tail -2 f1.txt
19) Просмотреть содержимое длинного файла (команда less) изучите как она работает
> less f1.txt
20) Вывести дату и время
> date

## Задание *
1) Отправить http запрос на сервер.
http://162.55.220.72:5005/terminal-hw-request 

> curl http://162.55.220.72:5005/terminal-hw-request <br/>
> curl "http://162.55.220.72:5005/get_method?name=Anastasiya&age=35"

2) Написать скрипт который выполнит автоматически пункты 3, 4, 5, 6, 7, 8, 13

> touch d:/myscript <br/> 
> cat >> d:/myscript

        #!/bin/bash
        # go to folder
        cd hw
        # create three folders
        mkdir a b c
        #  go to any folder
        cd a
        # create five files(3 txt, 2 json)
        touch f1.txt f2.txt f3.txt f4.json f5.json
        # create three folders
        mkdir a1 a2 a3
        # list the contents of a folder
        la -la
        # move any two files to any other folder
        cd ../
        mv a/{f4.json,f5.json} b
        Enter
        Ctrl+C
        cd ../
        chmod +x filename
        ./myscript
