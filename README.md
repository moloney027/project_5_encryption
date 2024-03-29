# Задание по шифрованию

Схема шифрования Вижинера.

Таблица Вижинера представляет собой квадратную матрицу с n^2 элементами, где n — число символов используемого алфавита. Каждая строка получена циклическим сдвигом всего алфавита на один символ.

Для шифрования выбирается буквенный ключ, в соответствии с которым формируется рабочая матрица шифрования.

Из полной таблицы выбирается первая строка и те строки, первые буквы которых соответствуют буквам ключа. Первой размешается первая строка, а под нею — строки, соответствующие буквам ключа в порядке следования этих букв в ключе.

1) под каждой буквой шифруемого текста записываются буквы ключа. Ключ при этом повторяется необходимое число раз;

2) каждая буква шифруемого текста заменяется по подматрице Вижинера буквами, находящимися на пересечении линий, соединяющих буквы шифруемого текста в первой строке подматрицы и находящихся под ними букв ключа;

Расшифровка текста производится в следующей последовательности:

1) над буквами зашифрованного текста последовательно надписываются буквы ключа, причем ключ повторяется необходимое количество раз.

2) в строке подматрицы Вижинера, соответствующей букве ключа, отыскивается буква, соответствующая знаку зашифрованного текста. Находящаяся под ней буква первой строки подматрицы и будет буквой исходного текста.

Задание состоит в написании программы для шифрования текста по схеме Вижинера. Текст для шифрования и ключ должны быть в русской кодировке и вводиться в диалоговом режиме.
