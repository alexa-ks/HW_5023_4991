# Руководство пользователя по работе с *Git*

*Git* — распределённая система управления версиями. Официальную документацию для работы с git можно найти по ссылке https://git-scm.com/doc.

## Основные команды

* git init - команда для инициализации репозитория (от англ. **repository** — хранилище)
* git add file_name.file_extension - команда для добавления файла с именем **file_name** и расширением **file_extension**, который *Git* будет отслеживать
* git commit - команда, которая делает для проекта снимок текущего состояния изменений, добавленных в раздел проиндексированных файлов
    - git commit -m "Комментарий к коммиту" - позволяет добавить комментарий к коммиту
    - git commit -am "Комментарий к коммиту" - создает коммит всех проиндексированных изменений и добавляет к коммиту подставленный комментарий.
* git diff - команда, которая инициирует функцию сравнения источников данных *Git* — коммитов, веток, файлов и т. д.
* git log - команда, которая отображает отправленные снимки состояния и позволяет просматривать и фильтровать историю проекта, а также проводить поиск по ней.
* git checkout - команда, которая получать старые коммиты и прежние версии файлов и осуществлять навигацию по существующим веткам.


## Команды для ветвления и слияния веток

**Branch** (англ.) — ветка.

* git branch - команда, которая отображает список веток в репозитории
    - git branch branch_name - команда, которая создает ветку с именем branch_name
    - git branch -d branch_name - команда, которая удаляет ветку с именем branch_name

* git merge branch_name - команда, которая объединяет ветки, при этом **branch_name** — название ветки, которая будет объединена с принимающей веткой
* git log --graph - команда, которая позволяет просмотреть историю коммитов в виде графика для текущей ветки

## Команды для работы с github

Ссылка на сайт https://github.com/

* git clone - команда, которая создаёт новый каталог, переходит внутрь и выполняет git init для создания пустого репозитория, затем она добавляет новый удалённый репозиторий (git remote add) для указанного URL (по умолчанию он получит имя origin), выполняет git fetch для этого репозитория и, наконец, извлекает последний коммит в ваш рабочий каталог, используя git checkout.
* git pull - команда, которая используется для извлечения и загрузки содержимого из удаленного репозитория
* git push - команда, которая используется для установления связи с удалённым репозиторием, вычисления локальных изменений отсутствующих в нём, и собственно их передачи в вышеупомянутый репозиторий. Этой команде нужно право на запись в репозиторий, поэтому она использует аутентификацию.