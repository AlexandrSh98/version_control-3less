# Подсказка по гиту

## Инициализация репозитория

```sh
git init
```

## Статус репозитория

```sh
git status
```

## Кэширование учётных данных
```sh
git config --global credential.helper cache
```

## Добавление отдельных файлов или всех файлов в область подготовленных файлов

Добавить отдельный файл в область подготовленных файлов можно параметром add с указанием имени файла. Просто замените somefile.js на актуальное имя.

```sh
git add somefile.js
```
Кроме того, можно добавить все файлы и папки в эту область, предоставив wildcard . вместо имени файла:
```sh
git add .
```
## Проверка статуса репозитория

Просмотреть статус нужного репозитория можно по ключевому слову status: его действие распространяется на подготовленные, неподготовленные и неотслеживаемые файлы.
```sh
git status
```

## Внесение изменений однострочным сообщением или через редактор

При создании коммита в репозитории можно добавить однострочное сообщение с помощью параметра commit с флагом -m. Само сообщение вводится непосредственно после флага, в кавычках.
```sh
git commit -m "Your short summary about the commit"
```
Также можно открыть текстовый редактор в терминале для написания полного сообщения коммита. Оно может состоять из нескольких строк текста, в котором подробно характеризуются изменения, внесённые в репозиторий.
```sh
git commit
```
## Просмотр истории коммитов с изменениями

Просматривать изменения, внесённые в репозиторий, можно с помощью параметра log. Он отображает список последних коммитов в порядке выполнения. Кроме того, добавив флаг -p, вы можете подробно изучить изменения, внесённые в каждый файл.
```sh
git log -p
```

## Просмотр заданного коммита

Просмотреть полный список изменений, внесённых конкретным коммитом, можно с помощью параметра show, указав идентификатор или хеш коммита. Значение хеша уникально для каждого коммита, созданного в вашем репозитории.
```sh
git show 1af17e73721dbe0c40011b82ed4bb1a7dbe3ce29
```
Также можно использовать сокращённый хеш.
```sh
git show 1af17e
```
