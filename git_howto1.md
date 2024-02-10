# Git
 ### ***Распределённая система управления версиями***

# Команды вводимые в системе Git

## Команда
```sh
 git init 
```
**Cоздает новый репозиторий Git**. С ее помощью можно преобразовать существующий проект без управления версиями в репозиторий Git или инициализировать новый пустой репозиторий. Большинство остальных команд Git невозможно использовать без инициализации репозитория, поэтому данная команда обычно выполняется первой в рамках нового проекта


## Команда
```sh
git add <
```
 **Добавляет изменение из рабочего каталога в раздел проиндексированных файлов**. Она сообщает Git, что вы хотите включить изменения в конкретном файле в следующий коммит. Однако на самом деле команда git add не оказывает существенного влияния на репозиторий: изменения регистрируются в нем только после выполнения команды git commit.

## Команда
```sh
git commit - m "Message"
```
**Git commit - это команда для записи индексированных изменений в репозиторий Git.**
Прежде чем создавать очередной коммит, необходимо проиндексировать файлы в рабочей области с помощью команды git-add. Новый коммит будет включать текущие состояния индексированных файлов плюс последние сохраненные состояния неиндексированных (но отслеживаемых) файлов.

## Команда
 ```sh
 git log
 ```
  **Oтображает отправленные снимки состояния и позволяет просматривать и фильтровать историю проекта, а также искать в ней конкретные изменения.** С помощью git status можно просматривать рабочий каталог и раздел проиндексированных файлов, в то время как git log показывает только историю коммитов.

## Команда
 ```sh
 git log --oneline
 ```
 **Выводит именно короткий хэш. Для других операций с коммитами достаточно использовать первые 4 символа.**
  Например, 3 команды ниже покажут содержимое одного и того же коммита $ git show 051f75475cb1dca3cd08c1c7367a3308671ccf7b $ git show 051f754 $ git show 051f Copy. История коммитов в PhpStorm. В окне Local Changes, на вкладке Log показывается вся история коммитов, в левой половине вкладки

## Команда
 ```sh
 git checkout <имя ветки>
 ```

 **Позволяет переключаться между последними коммитами (если упрощенно) веток: git checkout some-other-branch.** Создаёт ветку, в которую и произойдет переключение: git checkout -b some-other-new-branch. Если в текущей ветке были какие-то изменения по сравнению с последним коммитом в ветке (HEAD), то команда откажется производить переключение, дабы не потерять произведенную работу.

## Команда
```sh
git status
```
**Oтображает состояние рабочего каталога и раздела проиндексированных файлов.** С ее помощью можно проверить индексацию изменений и увидеть файлы, которые не отслеживаются Git. Информация об истории коммитов проекта не отображается при выводе данных о состоянии. Для этого используется команда git log. git tag Теги — это ссылки, указывающие на определенные точки в истории Git.

## Команда
```sh
git diff
```
**Сравнение — это функция, анализирующая два входных набора данных и отображающая различия между ними.** git diff представляет собой многоцелевую команду Git, которая инициирует функцию сравнения источников данных Git — коммитов, веток, файлов и т. д. В этом документе описываются типичные варианты вызова git diff и схемы рабочего процесса сравнения.

## Команда
```sh
git restore
```
**Kак и следует из ее названия, служит для восстановления файлов.** Команда позволяет восстанавливать файлы, но при этом четко показывает откуда и куда будут применяться изменения.

## Команда
```sh
git branch
```
**Это команда Git для управления ветками.** Используйте эту метку для обозначения всех вопросов, связанных с ветками, их созданием, структурой, управлением и удалением. Общие сведения. git branch – это команда для управления ветками в репозитории Git. Ветка в Git'е — это просто «скользящий» указатель на один из коммитов. Когда вы создаёте новые коммиты, указатель ветки автоматически сдвигается вперёд, к вновь созданному коммиту.

## Команда
```sh
git branch <имя ветки>
```
**Это команда Git для управления ветками.** команда для создания новых веток.

## Команда
```sh
git branch -d <имя ветки>
```
**Это команда Git для управления ветками.** Kоманда для удаления ненужных веток.

## Команда
```sh
git merge <имя ветки>
```
**Слияние — обычная практика для разработчиков, использующих системы контроля версий.** Независимо от того, созданы ли ветки для тестирования, исправления ошибок или по другим причинам, слияние фиксирует изменения в другом месте. Слияние принимает содержимое ветки источника и объединяет их с целевой веткой. В этом процессе изменяется только целевая ветка. История исходных веток остается неизменной.

## Команда
```sh
git log --graph 
git log --oneline --graph
```
**--graph` в команде `git log` позволяет просматривать журнал git в виде графика.**
Это может быть полезно, чтобы получить обзор того, как объединялись коммиты и как создавалась история git.

## Команда
```sh
git clone
```
**Kопирует существующий репозиторий Git.** Она похожа на команду SVN checkout, но имеет некоторые отличия: так, полученная «рабочая копия» представляет собой полноценный репозиторий Git с собственной историей и файлами, полностью обособленный от исходного репозитория..

## Команда
```sh
git pull
```
**Используется для извлечения и загрузки содержимого из удаленного репозитория и немедленного обновления локального репозитория этим содержимым.** Слияние удаленных вышестоящих изменений в локальный репозиторий — это обычное дело в процессе совместной работы на основе Git. Команда git pull на самом деле представляет собой комбинацию двух других команд: git fetch и git merge.

## Команда
```sh
Git push
```
**Это одна из консольных команд Git.** Она позволяет передать изменения из локального репозитория (набора файлов из папки .git) в удаленный. Разработчики используют эту команду в следующих целях:
добавить новый функционал в основную ветку
исправить баг
закрыть уязвимость в коде и др

# Остальное

>И конечно цитата:
>>Добавить ссылки,картинки и т.п.

**Без комментариев** [https://gb.ru/]

