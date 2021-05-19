# Базовые действия в HDFS

Необходимо написать bash скрипт `hdfs_test.sh` выполняющий следующую последовательность действий на namenode Hadoop кластера:  
1. Создать локально файл test.txt размером 100Мб
2. Создать hdfs-директории temp и logs
3. Записать файл test.txt в директорию temp
4. Посмотреть свойства записанного файла
5. Переместить файл test.txt в директорию logs
6. Установить фактор репликации для файла равным 1
7. Скопировать test.txt в test2.txt
8. Скопировать директорию logs в logs2 с помощью hadoop distcp
9. Установить права доступа, означающие чтение и запись только для владельца для файла test2.txt в директории logs2
10. Вывести свойства всех файлов в logs2
11. Посмотреть размер всех директорий в /
12. Удалить директорию logs
13. Запустить fsck на директории logs2
14. Посмотреть отчет о HDFS через dfsadmin
15. Переместить /logs2/test2.txt в локальную папку /
16. Добавить содержимое локального файла test2.txt в конец файла /logs2/test.txt в hdfs
17. Вывести размер файлов в /logs2 в Mb

В качестве ответа нужно прислать сам скрипт `hdfs_test.sh` и весь его вывод в виде текстового файла `hdfs_test_results.txt`.