# Домашнее задание №3 (дополненное)
Создание инструкции в программе Git и использованию языка Markdown
___
## ВАЖНО. 
### Общее

Git — система контроля версий (файлов). Что-то вроде возможности сохраняться в компьютерных играх (в Git эквивалент игрового сохранения — коммит). **Важно**: добавление файлов к «сохранению» двухступенчатое: сначала добавляем файл в индекс (`git add`), потом «сохраняем» (`git commit`).

Любой файл в директории существующего репозитория может находиться или не находиться под версионным контролем (отслеживаемые и неотслеживаемые).

### Простейший цикл работ

- Редактирование, добавление, удаление файлов (собственно, работа).
- Индексация/добавление файлов в индекс (указание для git какие изменения нужно будет закоммитить).
- Коммит (фиксация изменений).
- Возврат к шагу 1 или отход ко сну.
___


# Выделение #
Курсив обозначается *звездочками* "*" или _подчеркиванием_ "_".
Полужирный шрифт - двойными **звездочками** "**" или __подчеркиванием__ "__".
Соответственно комбинированное выделение **звездочками и _подчеркиванием_**.
Для зачеркнутого текста используются две тильды "~~". ~~Уберите это.~~

___
## Списки ##

Markdown поддерживает два вида списков: маркерованный (ненумированный) и нумерованный. 

Нумированный список делается простым проставлением цыфр с точкой в начале строки. Номер не имеет значения, нужно чтобы это была просто любая цифра. Вот так:

1. Первый пункт нумерованного списка
2. Второй пункт нумированного списка
10. Тут в начале строки использована 10 но отображается 3.
 

Для организации маркерованного (ненумированного) списка используются знаки *, + и -. В любом случае вид маркера будет одинков. Вот так:

* использование звездочки "*"
- Или минуса "-"
+ Или плюса "+"

Чтоб сделать многоуровневый список, нужно будет сделать отступы (4 или 8 пробелов). Внутри пунктов списка можно вставить абзацы с таким же отступом. Обратите внимание на пустую строку выше и на пробелы в начале (нужен по меньшей мере один).  

    Чтобы вставить разрыв строки, но не начинать новый параграф, нужно добавить два пробела перед новой строкой. Этот текст начинается с новой строки, но находится в том же абзаце.  

1. Первый пункт.
   * Ненумерованный вложенный список.
2. Второй пункт. 
   1. Нумерованный вложенный список
   1. ...
   2. ....
   
3. И еще один пункт.

Не понял как делать многоуровневые нумерованные спики чтобы подпункты отобрадали цыфры верхнего уровня типа 2.1. или 4.4.


___

## Ссылки ##

Ссылки можно оформить разными способами. Для этого отображаемый текст обрамляется квадратными скобками [], а сам адрес ссылки заключается в круглые скобки (). Вот так:  

[Обычная ссылка в строке](https://gb.ru/)

Если есть желание сделать так, чтобы при наведении на ссылку появляось всплывающее сообщение, то после адреса ссылки через пробел вводится елаемый текст, который заключается в кавычки "".  Вот так:   
[Обычная ссылка с title](https://gb.ru/ "Сайт GeekBrains")

Кроме того, если Вы хотите показать активную ссылку полностью в тексте, то можно обрамить ее значками <>. Вот так:  
<support@geekbrains.ru>

___
## Цитаты #

 Цитаты вводятся при использовании в начале строки символа ">" 
> Цитатами очень удобно обозначать исходный текст письма или обращения.
> Эта строка - часть той же цитаты.

Разрыв цитаты.

> Это очень длинная строка, но она будет правильно процитирована даже при размещении на нескольких строках. Продолжаем писать, чтобы эта строка не вмещалась на одной строке в любом окне. Кстати, в цитаты можно *вставлять* даже **Markdown**.  
>  1. Списки и любые другие элементы   
>      * даже многоуровневые...
___


## Горизонтальные линии #

Горизонтальные линии делаются при вводе троных символов

Дефисы "-"

Звездочки "*"

Подчеркивания "_"
___

***

---


___

## Таблицы

Таблицы не являются частью Markdown, но многие обработчики, например Markdown Here и Github, поддерживают их.

При наборе таблицы столбца образуются при использовании символа вертикальной черты (|). Заголовой таблицы образуется если испольовать символ (-).  Вертикальные линии обозначают столбцы, хоть и не отображаются. Внешние вертикальные линии (|) не обязательны, и они нужны только чтобы сам код Markdown выглядел красиво.

| Таблицы       | Это                | Стремно |
| ------------- |:------------------:| -----:|
| столбец 3     | выровнен вправо    | 1600 |
| столбец 2     | выровнен по центру |   12 |
| зебра-строки  | прикольные         |   1 |

По умолчанию выравнивание в таблице происходит влево. Для выравнивания вправо в каком то столбце в строке, которая отвечает за шапку в таблице, используется символ двоеточия (:). Для выравнивания по центру (:) с начале и  конце столбца.

В остальном это геморой - верстать таблице в Markdown.


# Инструкция: заливаем проект на GitHub

1. Создание локального репозитория и добавление файлов в локальный репозиторий.
    `git init` и `git add` наше все
    Для того чтобы создать свой локальный репозиторий, необходимо выбрать необходимую директорию через команду `cd` "адрес директории", после чего ввести `git init`, после чего все другие команды git (такие как `add, commit, branch` и т.д.) начнут опозноваться и выполняться. После можно спокойно работать с имеющимися файлами в репозитории (вашей папке) и записывать их изменения через `commit -m "Название сохранения"`, сохраняя их в `log`.   
    
2. Создание версии проекта на стационарном компе. Творим...)))
3. Создание репозитория на Github   
   Если мы хотим иметь возможность сохранения проекта в интернете, создадим репозиторий на Github. Для начала нужно зарегистрироваться на сайте github.com 
   После регистрации нажимаем кнопочку "+" и вводим название репозитория. Выбираем тип Public (репозиторий всегда Public для бесплатной версии) и нажимаем Create.
   В результате мы создали репозиторий на сайте Github. На экране мы увидим инструкцию, как соединить наш локальный репозиторий со вновь созданным. Часть команд нам уже знакома.   
   
   Скопировать и вставить указанные команды в командную строку консоли на компе. В итоге мы "подружим" локальную версию и GitHub   
   
   `git remote add github ...(адрес репозитория на GitHub)`   
   
   Следующей командой вы занесете все изменения, которые были сделаны в локальном репозитории на Github.   
   
   `git push -u github master`   
   
   Ключ -u используется для того, чтобы установить связь между удаленным репозиторием github и вашей веткой master. Все дальнейшие изменения вы можете переносить на удаленный репозиторий упрощенной командой.   
   
   `git push`   
   
   
4. Вуаля весь Ваш проект теперь на GitHub, где вы можете продолжить работа над ним.
5. Возможен перенос репозитория с GitHub на другой (не ваш) компьютер.   

   После того, как репозиторий был создан на Github, его можно скопировать на любой другой компьютер. Для этого применяется команда:   
   
   `git clone`   
   
   Но это уже совсем другая история.

