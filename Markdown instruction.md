# Инструкция для работы с Markdown 

## Выделение текста

Чтобы выделить текст курсивом необходимо обрамить его звездочками (*) или (_) Например, *вот так*, или _вот так_.

Альтернативные способы выделения текста жирным или курсивом нужны для того, чтобы мы могли совмещать оба этих способа. Например, _текст может быть выделен курсивом и при этом быть **полужирным**_. 

Чтобы выделить текст полужирным, необходимо обрамить его двумя звездочками (**).

### Списки

Чтобы выделить нумерованный список необходимо

1. Первый пункт
2. Второй пункт 

Для разметки неупорядоченных списков можно использовать или `*`, или `-`, или `+`:

Чтобы добавить ненумерованные списки, необходимо пункты выделить звездочкой (*). 
Например, вот так:

* Элемент 1
* Элемент 2
* Элемент 3

На самом деле не важно как в коде пронумерованы пункты, главное, чтобы перед элементом списка стояла цифра (любая) с точкой. Можно сделать и так:

0. элемент 1
0. элемент 2
0. элемент 3
0. элемент 4

Вложенные пункты создаются четырьмя пробелами перед маркером пункта:

* элемент 1
* элемент 2
    * вложенный элемент 2.1
    * вложенный элемент 2.2
* элемент ...

## Список с абзацами: 

* Раз абзац. Lorem ipsum dolor sit amet, consectetur adipisicing elit.
* Два абзац. Donec sit amet nisl. Aliquam semper ipsum sit amet velit. Suspendisse id sem consectetuer libero luctus adipiscing.
* Три абзац. Ea, quis, alias nobis porro quos laborum minus sed fuga odio dolore natus quas cum enim necessitatibus magni provident non saepe sequi?
    Четыре абзац (Четыре пробела в начале или один tab).

# Изображения

Чтобы вставить изображение в текст, достаточно написать следующее: ![]() 

Например:

![Привет, это ЗК!](koleos.jpg)


## Работа с таблицами

## Цитаты

**Цитаты оформляются как в емейлах, с помощью символа `>`.**

> This is a blockquote with two paragraphs. Lorem ipsum dolor sit amet,
> consectetuer adipiscing elit. Aliquam hendrerit mi posuere lectus.
> Vestibulum enim wisi, viverra nec, fringilla in, laoreet vitae, risus.
> 
> Donec sit amet nisl. Aliquam semper ipsum sit amet velit. Suspendisse
> id sem consectetuer libero luctus adipiscing.

**Или более ленивым способом, когда знак `>` ставится перед каждым элементом цитаты, будь то абзац, заголовок или пустая строка:**

> This is a blockquote with two paragraphs. Lorem ipsum dolor sit amet,
consectetuer adipiscing elit. Aliquam hendrerit mi posuere lectus.
Vestibulum enim wisi, viverra nec, fringilla in, laoreet vitae, risus.
>
> Donec sit amet nisl. Aliquam semper ipsum sit amet velit. Suspendisse
id sem consectetuer libero luctus adipiscing.

**В цитаты можно помещать всё что угодно, в том числе вложенные цитаты:**

> ## This is a header.
>
> 1.   This is the first list item.
> 2.   This is the second list item.
>
> > Вложенная цитата.
>
> Here's some example code:
>
>     return shell_exec("echo $input | $markdown_script");

### Исходный код

    В чистом Маркдауне блоки кода отбиваются 4 пробелами в начале каждой строки.

    Но в GitHub-Flavored Markdown (сокращенно GFM) есть более удобный способ: ставим по три апострофа (на букве Ё) до и после кода. Также можно указать язык исходного кода.

```html
<nav class="nav nav-primary">
  <ul>
    <li class="tab-conversation active">
      <a href="#" data-role="post-count" class="publisher-nav-color" data-nav="conversation">
        <span class="comment-count">0 комментариев</span>
        <span class="comment-count-placeholder">Комментарии</span>
      </a>
    </li>
    <li class="dropdown user-menu" data-role="logout">
      <a href="#" class="dropdown-toggle" data-toggle="dropdown">
        <span class="dropdown-toggle-wrapper">
          <span>
            Войти
          </span>
        </span>
        <span class="caret"></span>
      </a>
    </li>
  </ul>
</nav>
```
    Самое приятное, что в коде не нужно заменять угловые скобки `< >` и амперсанд `&` на их html-сущности.

### Инлайн код

    Для вставки кода внутри предложений нужно заключать этот код в апострофы (на букве Ё). 

    Пример:

 `<html class="ie no-js">`.

    Если внутри кода есть апостроф, то код надо обрамить двойными апострофами: 

``There is a literal backtick (`) here.``

### Горизонтальная черта

`hr` создается тремя звездочками или тремя дефисами.

***

## Ссылки  (_**Спросить может здесь ошибка в описании у меня?**_)

* Это встроенная [ссылка с title элементом](http://example.com/link "Я ссылка").

* Это — [без title](http://example.com/link).

А вот [пример][1][нескольких][2] [ссылок][id] с разметкой как у сносок. Прокатит и [короткая запись][] без указания id.

    [1]: http://example.com/ "Optional Title Here"

    [2]: http://example.com/some

    [id]: http://example.com/links (Optional Title Here)

    [короткая запись]: http://example.com/short

_Вынос длинных урлов из предложения способствует сохранению читабельности исходника. Сноски можно располагать в любом месте документа._

## Команды

_**git init**_

>Эта команда создаёт в текущем каталоге новый подкаталог с именем .git, содержащий все необходимые файлы репозитория — структуру Git репозитория. На этом этапе ваш проект ещё не находится под версионным контролем. 

>Если вы хотите добавить под версионный контроль существующие файлы (в отличие от пустого каталога), вам стоит добавить их в индекс и осуществить первый коммит изменений. Добиться этого вы сможете запустив команду git add несколько раз, указав индексируемые файлы, а затем выполнив git commit:

_**git add**_

>Команда git add добавляет содержимое рабочего каталога в индекс (staging area) для последующего коммита. По умолчанию git commit использует лишь этот индекс, так что вы можете использовать git add для сборки слепка вашего следующего коммита.

_**git status**_

>Команда git status показывает состояния файлов в рабочем каталоге и индексе: какие файлы изменены, но не добавлены в индекс; какие ожидают коммита в индексе. Вдобавок к этому выводятся подсказки о том, как изменить состояние файлов.

_**git commit**_

>Команда git diff используется для вычисления разницы между любыми двумя Git деревьями. Это может быть разница между вашей рабочей копией и индексом (собственно git diff), разница между индексом и последним коммитом (git diff --staged), или между любыми двумя коммитами (git diff master branchB).

_**git log**_

>После того, как вы создали несколько коммитов или же клонировали репозиторий с уже существующей историей коммитов, вероятно вам понадобится возможность посмотреть что было сделано — историю коммитов. Одним из основных и наиболее мощных инструментов для этого является команда git log.

_**git checkout**_

>После того как вы нашли ссылку на нужный коммит в истории, для перехода к нему можно использовать команду git checkout. Команда git checkout — это простой способ «загрузить» любой из этих сохраненных снимков на компьютер разработчика.

_**git checkout master**_

>переключение на ветку master в последний коммит

_**git diff**_

>Показывает различия между проиндексированной и последней зафиксированной версиями файлов

**git diff [первая ветка]...[вторая ветка]**

>Показывает разницу между содержанием коммитов двух веток

_**git show [коммит]**_

>Выводит информацию и показывает изменения в выбранном коммите

_**git branch**_

>Список именованных веток коммитов с указанием выбранной ветки

_**git branch [имя ветки]**_

>Создаёт новую ветку

_**git merge [имя ветки]**_

>Вносит изменения указанной ветки в текущую ветку

_**git branch -d [имя ветки]**_

>Удаляет выбранную ветку


## Заголовки

Заголовки отмечаются диезом `#` в начале строки, от одного до шести. Например:

# Заголовок первого уровня #

## Заголовок h2

### Заголовок h3

#### Заголовок h4

##### Заголовок h5

###### Заголовок h6

В декоративных целях заголовки можно «закрывать» с обратной стороны.

### Emphasis

>Выделять слова можно при помощи `*` и `_`. Один символ для наклонного текста, два символа для жирного текста, три — для наклонного и жирного одновременно.

Например, это _italic_ и это тоже *italic*. А вот так уже __strong__, и так тоже **strong**. А так ***жирный и наклонный*** одновременно.

### Зачеркивание

>В GFM добавлено зачеркивание текста: две тильды `~` до и после текста.

Например: ~~Зачеркнуто~~

### Таблицы

Вы можете создавать таблицы с вертикальной чертой | и дефисами -. Дефисы используются, чтобы создать для каждого столбца заголовок. Вертикальные черты разделяют столбцы. Необходимо включить пустую строку перед таблицей, чтобы она правильно преобразовалась для просмотра.

| First Headef | Second Header |
| --- | --- |
| Content Cell | Content Cell  |

# Локальная работа с файлами
> Теперь поработаем с этими файлами локально. Можно посмотреть, например, на текущий
статус. Нажимаем Enter и видим ту же фатальную ошибку. Разберёмся, почему возникает
такая ошибка.

> Обратите внимание, что в последней строке указано, кто выполняет операции. То есть здесь
указан мой аккаунт и указан компьютер, на котором я работаю. Затем идёт папка, в которой
мы находимся.

> Сейчас команда git status запускается в папке Lesson 3, но в ней нет репозитория. В папке
Lesson 3 есть другая папка, где уже лежит репозиторий. Поэтому чтобы с Git работать
аккуратно, надо поместить всё в папку version_control_lection_3. В разных операционных
системах это делается по-разному. В Linux и Mac, чтобы поменять местоположение,
выполняется команда cd — change directory — поменять директорию. Далее надо просто
указать, куда перейти. Перейдём в папку version_control_lection_3.

> Обратите внимание, что выдача терминала поменялась. Там, где раньше было написано Lesson
3, теперь указано имя нашего репозитория. И если сейчас мы запустим команду git status, то
увидим уже знакомую выдачу. У нас есть информация, что мы находимся на ветке master и
нам не надо ничего коммитить. Соответственно, можно спокойно продолжать работу.

> Посмотрим, что хранится в нашем репозитории. Для этого снова очистим выдачу терминала и
посмотрим на сами файлы. Файл Teftelka здесь нет, но есть текст, замещающий его.

> В тексте есть картинка. У нас есть информация, что здесь должна быть Тефтелька, но, так как
самого файла в репозитории нет, мы видим не фотографию, а замещающий текст. Можно
посмотреть на лог изменений и увидеть:
* какие изменения происходили;
* какие коммиты были в этом файле, когда и кем сделаны;
* и что вообще происходило.

То есть вся история здесь есть.

Мы можем:

* перемещаться по всем коммитам;
* переходить с одного на другое;
* проследить, как выполнялась работа;
* посмотреть на лог в виде графа;
* посмотреть, есть ли ветки, и если есть, то как осуществлялась работа.
> Обратите внимание, что последние два коммита уже сделаны в одной ветке, до этого было
слияние с разрешением конфликта версий. Наблюдается также расхождение, когда
стартовала другая ветка. То есть можно посмотреть всю историю работы над этим файлом.

> По факту у вас появляется полная копия представленной работы, будто вы делали её
самостоятельно. То есть вся история у вас есть. Вы можете остановиться, продолжить работу с
этим файлом, и у вас появится собственная версия репозитория. Однако всё происходит
локально. С версией, которая находится на GitHub, она не связана.

> Мы рассмотрели второй способ создания репозиториев. Первый способ осуществлялся через
git init, когда мы создавали собственный репозиторий. Второй способ реализуется через git
clone: мы можем взять чужой репозитории, который, кстати, тоже был когда-то создан через
git init, но продолжить работу с ним уже локально.
# Практика
> Работа с сайтом github.com
Посмотрим, как всё работает на практике. Для начала создадим папку на нашем рабочем
столе. Назовём её Lesson 3 и откроем в редакторе VS Code. Так мы начинали все лекции, но
создавали локальный репозиторий с использованием git init. Теперь поступим несколько
иначе, не будем создавать свой репозиторий, а возьмём готовый. Для этого перейдём на сайт
github.com. Практически все, так или иначе, знакомы с этим сайтом, как минимум слышали о
нём.

> На этом сайте есть поиск. Вы можете находить здесь разных авторов и проекты. Посмотрим на
один из готовых репозиториев.

> В этот репозиторий я добавил файлы второй лекции. Скачаем их так, чтобы на нашем
компьютере они стали локальным репозиторием.

> Эти файлы можно посмотреть и на самом сайте. Открывая их, можно увидеть, как они
выглядят в редакторе после обработки Markdown. Есть, например, файл .gitignore, здесь мы,
соответственно, игнорируем нашу Тефтельку. И есть зелёная кнопка Code. Если мы нажмём на
неё, появится строка с адресом. Здесь написано Use Git or checkout with SVN. SVN — это
системы контроля версий.

> Скопируем эту строку и перейдём в код. Выберем строку HTTPS, нажмём «Копировать», и
после этого нам понадобится новая команда внутри VS Code. Откроем терминал. В терминале
дадим новую команду Git: скажем git clone и укажем тот адрес, который скопировали.

> После этого Git скопирует репозиторий, находящийся на сервисе GitHub, в наш локальный
репозиторий. То есть на нашем компьютере появится полная копия этого репозитория. Но
прежде чем мы это сделаем, сначала вызовем команду git status. Убедимся, что Cit не
настроен. Появилась надпись, что это не Git-репозиторий, возникла какая-то фатальная
ошибка, и наша программа отказывается работать дальше. То есть мы убедились, что здесь
лежит пустая папка без каких-либо репозиториев.

> Снова вызовем команду git clone. Вставим туда скопированный адрес и нажмём на Enter.
Внутри папки Lesson 3 появилась новая папка с именем version_control_lection_3. Узнаем,
почему у неё такое название.

> Дело в том, что сам репозиторий на GitHub называется именно так. То есть Git скачал
репозиторий, который находился на GitHub, создал папку с таким же названием и поместил
всё, что находилось в репозитории. Обратите внимание, внутри этой папки есть файл .gitignore
и файл Markdown instruction.md. Именно эти файлы находились в нашем репозитории на сайте
GitHub.

# GitHub

