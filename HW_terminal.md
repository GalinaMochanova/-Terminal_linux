Linux terminal(Gitbash)
======================

1) Посмотреть где я

        pwd

2) Создать папку 
 
       mkdir group_28
3) Зайти в папку
 
       cd group_28
4) Создать 3 папки
 
       mkdir dir_1 dir_2 dir_3
5) Зайти в любоую папку
 
       cd dir_1
6) Создать 5 файлов: (3 txt, 2 json)
 
       touch test_1.txt test_2.txt test_3.txt test_4.json test_5.json
7) Создать 3 папки 
 
       mkdir folder_1 folder_2 folder_3
8) Вывести список содержимого папки
 
       ls -la
       
9) Открыть любой txt файл
 
         vim test_1.txt
         
10) Написать туда что-нибудь, любой текст
 ```
       vim test_1.txt
       
       i
       
       {
       "name": "galina",
       "year": 1990,
       "month": 3,
       "day":3
        }
 ```
11) Cохранить и выйти
``` 
     esc
     :wq
     +enter
```

12) Выйти из папки на уровень выше
 
         cd ..
      
13) Переместить любые 2 файла, которые вы создали, в любую другую папку
``` 
mv test_1.txt folder_1/test_1.txt
mv test_2.txt folder_1/test_2.txt
```
14) Скопировать любые 2 файла, которые вы создали, в любую другую папку
```
cp test_3.txt folder_2/test_3.txt
cp test_4.json folder_3/test_4.json
```
15) Найти файл по имени
 
          find . -name "test_1.txt"
16) Просмотреть содержимое в реальном времени
 
        tail -f test_3.txt
17) Вывести несколько первых строк из текстового файла
```
head -n3 test_5.json

{
        "name":"galina",
        "year": 1990,
 ```

18) вывести несколько последних строк из текстового файла
``` 
   tail -n3 test_6.json
   
        "month": 5,
        "day":3
}
```
19) просмотреть содержимое длинного файла: 
```
less test_6.json
q
```
20) вывести дату и время
 
        date
---

**Задание** *
1) Отправить http запрос на сервер
http://162.55.220.72:5005/object_info_3?name=Vadim&age=32&salary=1000 

       curl "http://162.55.220.72:5005/object_info_3?name=Vadim&age=32&salary=1000"


2) Написать скрипт который выполнит автоматически пункты 3, 4, 5, 6, 7, 8, 13
``` 
cd group_28; 
mkdir fold_1 fold_2 fold_3; 
cd fold_1; 
touch test_1.txt test_2.txt test_3.txt test_4.json test_5.json; 
mkdir inner_1 inner_2 inner_3; 
ls -la; 
mv {test_1.txt,test_2.txt} inner_1
```
