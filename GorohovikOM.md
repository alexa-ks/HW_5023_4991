# Руководство пользователя по работе с Git

## 1. Основные команды 
* git init  инициализирует репозиторий
* git add - добавляем файл в репозиторий
* git status - проверка статуса репозитория
* git commit -m "сообщение"- добавление комментарияя
* git commit -am - одновременное добавление файла в репозиторий и комментария к нему
* git log - просмотр всех версий файла
* git diff - просмотр изменений последнего сохранения
* git checkout - переход к другой версии файла

## Выделение текста

Чтобы выделить текст курсивом необходимо обрамить его звездочками (*) или знаком нижннго подчеркивания (_). Например, *вот так* или _так_.

Чтобы выделить текст полужирным необходимо обрамить его двойными звездочками (**) или знаком нижнего подчеркивания (_). Например, **вот так** или __так__.

Альтернативные способы выделения текста жирным или курсивом необходимы для того, чтобы мы могли совмещать оба этих способа. Например, _текст может быть выделен курсивом и при этом **быть полужирным**_.

Чтобы получить зачекркнутый текст необходимо обрамить его двумя знаками тильды (~~).
Например ~~вот так~~.

Чтобы получить подчекркнутый текст необходимо обрамить его тегами.
Например <u>вот так</u>.

Чтобы получить горизонтальную разделительную черту необходимо отметить тустую строку тремя звезжочками , тремя нижними подчеркиваниями или тремя тире. Приэтом между текстом и строкой располодения знаков должна быть пустая строка.
Например:

---

Первый текст

***
второй текст
___
Третий текст

## Списки

Чтобы добавить ненумерованный список, необходимо пункты выделить звездочкой (*), минумсом(-) или плюсиком (+).
Например вот так:
* Элемент 1
- Элемент 2
+ Элемент 3

Чтобы добавить нумерованный список, необходимо пункты просто пронумеровать. Главное чтобы первый пункт был под номером 1.
Например вот так:
1. Первый пункт
2. Второй пункт
7. Третий пункт
9. Четвертый пункт

## Работа с изображениями

Чтобы вставить изображение в текст, достаточно написать следующее:
![Привет, это мяч!](leto-boll.jpg)
В квадратных скобках пишется текст отображаемы в случае если картинка не загрузилась, в круглых скобках название файла с картинкой и путь к нему. 
## Цитаты
 Начало цитаты обозначается знаком одним больше >, если это цитата первого уровня 
Двумя >> если цитата второго уровня
Тремя >>> если цитата третьего уровня. И так далее...
Например:
># Так обозначается заголовок цитаты
> цитата первого уровня
>> цитата второго уровня

## Ссылки
Для оформления ссылки нкжно написать следующее: [Видимая часть, название ссылки] (http://roga-kopyta.ru.net адрес ссылки - невидимая часть)

[Мой сайт](http://roga-kopyta.ru.net)
Если заключить адрес в угловые скобки, то он автоматически станет ссылкой

<http:/roga-kopyta.ru.net>

## Заголовки
Начало заголовка следует начинать со знака решетка (#). Причем один такой знак означает что это заголовок первого уровня, два - второго и т.д. Как приме разметка этого руководства пользователя.

Заголовок первого уровня также можно выделить набрав на пустой строке, следующей за названием зоголовка хотя бы одного знака равно (=), для заголовка второго уровня знак минус (-).
Например: 

Заголовок первого уровня
=

Заголовок второго уровня
-

## 2. Работа с ветками
* git branch - показывает список веток
* git branch branch_name - создает ветку с именем branch_name
* git checkout branch_name - переключается на ветку с именем branch_name
* git checkout -b brabranch_name - создает ветку с именем branch_name и переключается на нее
* git merge branch_name -  производит слияние ветки branch_name с текущей веткой
* git checkout -d branch_name - удаляет ветку branch_name
* git log --graph - показывает лог всех веток одновременно
* git commit --amend -m "новое сообщение" - меняет комментарий к последнему коммиту.

## 3. Работа с удаленными репозиториями
git clone repositiry_adres - клонирует чужой удаленный репозиторий в локальный
fork - копия чужого репозитория
cd folder_name - переход в другую папку
git remote -v  - показывает к какому репозиторию на GitHub приязан локальный репозиторий
git push - выгрузить данные в удаленный репозиторий
git pull - загрузить данные с удаленного репозитория