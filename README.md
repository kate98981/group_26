# group_26
1) Посмотреть где я - pwd
2) Создать папку - mkdir folder_1
3) Зайти в папку - cd folder_1
4) Создать 3 папки - mkdir ../folder_2 ../folder_3 ../folder_4
5) Зайти в любоую папку - cd ../folder_3
6) Создать 5 файлов (3 txt, 2 json) - touch txt_1.txt txt_2.txt txt_3.txt json_1.json json_2.json
7) Создать 3 папки - mkdir folder_1 folder_2 folder_3
8. Вывести список содержимого папки - ls -la
9) + Открыть любой txt файл - 
	vim txt_1.txt
10) + написать туда что-нибудь, любой текст. 
	1. Клавиша "i"
	2. Ввод текста
	3. Клавиша "esc"
11) + сохранить и выйти. - :wq
12) Выйти из папки на уровень выше - cd ..
—
13) переместить любые 2 файла, которые вы создали, в любую другую папку.
	mv folder_3/txt_1.txt folder_3/txt_2.txt -t folder_2
14) скопировать любые 2 файла, которые вы создали, в любую другую папку.
	cp folder_3/json_1.json folder_3/json_2.json -t folder_2
15) Найти файл по имени - 
	find . -name terminal1.txt
16) просмотреть содержимое в реальном времени (команда grep) изучите как она работает. - 
	tail -f txt_1.txt
17) вывести несколько первых строк из текстового файла
	head txt_1.txt
18) вывести несколько последних строк из текстового файла
	tail txt_1.txt
19) просмотреть содержимое длинного файла (команда less) изучите как она работает.
	 less txt_2.txt
20) вывести дату и время
	date +"%D %T"
=========

Задание *
1) Отправить http запрос на сервер.
http://162.55.220.72:5005/object_info_3?name=Vadim&age=32&salary=1000
 curl "http://162.55.220.72:5005/object_info_3?name=Vadim&age=32&salary=1000"
2) Написать скрипт который выполнит автоматически пункты 3, 4, 5, 6, 7, 8, 13
#!/bin/bash
cd folder_1
mkdir f1 f2 f3
cd f1
touch t1.txt t2.txt t3.txt j1.json j2.json
mkdir f4 f5 f6
ls -la
mv t1.txt t2.txt -t ../f2
=====================
1) Отправить http запрос на сервер.
http://162.55.220.72:5005/terminal-hw-request
 curl "http://162.55.220.72:5005/terminal-hw-request"
