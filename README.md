Комманды git
============

___

_Список часто используемых комманд Git_


--

### Получение и создание проектов

| Комманда | Описание |
| ------- | ----------- |
| `git init` | Инициализация локального git репозитория |
| `git clone ssh://git@github.com/[username]/[repository-name].git` | Копирование удаленного git репозитория |

### Базовое управление снапшотами.

| Комманда | Описание |
| ------- | ----------- |
| `git status` | Проверка статуса |
| `git add [file-name.txt]` | Добавление файла в stage |
| `git add -A` | Добавление всех новых и изменненых файлов в stage |
| `git commit -m "[commit message]"` | Создание коммита со всеми изменениями |
| `git rm -r [file-name.txt]` | Удаление файла или каталога |

### Branching & Merging

| Комманда | Описание |
| ------- | ----------- |
| `git branch` | Список веток (астериском отмечена текущая ветка) |
| `git branch -a` | Список всех веток (Локальных и удаленных) |
| `git branch [branch name]` | Создание новой ветки |
| `git branch -d [branch name]` | Удаление ветки |
| `git push origin --delete [branch name]` | Удаление ветки на уделнном ресурсе |
| `git checkout -b [branch name]` | Создание новой ветки и переключение на нее |
| `git checkout -b [branch name] origin/[branch name]` | Клонирование удаленной ветки и переключение на нее |
| `git branch -m [old branch name] [new branch name]` | Переименование локальной ветки |
| `git checkout [branch name]` | Переключение на ветку |
| `git checkout -` | Переключение на ветку из которой в последний раз было выполнено переключение |
| `git checkout -- [file-name.txt]` | Сброс изменений в файл |
| `git merge [branch name]` | Обьединение ветки в активную ветку |
| `git merge [source branch] [target branch]` | Обьединение ветки в целевую ветку |
| `git stash` | Stash changes in a dirty working directory |
| `git stash clear` | Remove all stashed entries |

### Обновление проектов

| Комманда | Описание |
| ------- | ----------- |
| `git push origin [branch name]` | Отправка ветки в удаленный репозиторий |
| `git push -u origin [branch name]` | Отправка ветки в нелокальный репозиторий (с сохранением ветки) |
| `git push` | Отправка измененйи в нелокальный репозиторий (в сохраненную ветку) |
| `git push origin --delete [branch name]` | Удаление ветки на нелокальном репозитории |
| `git pull` | Обновление локального репозитория до последнего коммита |
| `git pull origin [branch name]` | Получение всех изменений из удаленного репозитоиия |
| `git remote add origin ssh://git@github.com/[username]/[repository-name].git` | Добавление удаленного репозитория |
| `git remote set-url origin ssh://git@github.com/[username]/[repository-name].git` | Изменение ссылки на удаленный репозиторий на тип SSH |

### Inspection & Comparison

| Комманда | Описание |
| ------- | ----------- |
| `git log` | Просмотр изменений |
| `git log --summary` | Просмотр измененений (детализированный) |
| `git log --oneline` | Просмотр изменений (сокращенный) |
| `git log --graph --oneline` | Отображение веток |
| `git diff [source branch] [target branch]` | Просмотр изменений перед обьединением |
