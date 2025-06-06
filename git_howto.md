# Подсказка по GIT(с урока)
Создание репозитория(инициализация):
```sh
git init
```

Добавление файла в индекс (подготовка к коммиту)

```sh
git add 
```

Фиксирование изменения из индекса в репозиторий (с комментарием)
```sh
git commit -m "Message"
```

Показывает историю коммитов (подробно)
```sh
git log
```

Сокращенная история (хеш+сообщение)
```sh
git log --oneline
```

Переключение между ветками/коммитами или откат файлов
```sh
git checkout
```

Показывает разницу (изменения) между рабочей директорией и индексом,
индексом и последним коммитом
```sh
git diff
```

Переключение на основную ветку
```sh
git checkout master
```

Клонирование существующего репозитория
```sh
git clone <url>
```

Проверка статуса
```sh
git status
```

# Ветвление и слияние
## Ветки
Ветки в Git позволяют параллельно вести разработку разных функций без interference с основным кодом.
Список веток
```sh
git branch
```
Создать новую ветку
```sh
git branch <name> 
```
Переключиться на ветку
```sh
git checkout <branch> 
```
Переключиться на ветку
```sh
git checkout -b <new-branch>
```
## Слияние
Слияние объединяет изменения из разных веток, разрешая возможные конфликты между версиями кода
Слить указанную ветку с текущей
```sh
git merge <branch> 
```
# 🔍 Просмотр истории
История коммитов в Git помогает отслеживать изменения, находить ошибки и понимать эволюцию проекта
Подробная история
```sh
git log 
```
Компактная история с визуализацией
```sh
git log --oneline --graph 
```
Показывает изменения
```sh
git diff 
```
# 🔄 Работа с удалёнными репозиториями
Удалённые репозитории синхронизируют локальную разработку с командной работой, используя push и pull.
Показать удалённые репозитории
```sh
git remote -v 
```
Отправить изменения
```sh
git push origin <branch>
```
Получить изменения
```sh
git pull origin <branch>
```
Получить изменения без слияния
```sh
git fetch 
```
# 🛠️ Полезные инструменты
.gitignore

```sh
# Игнорировать файлы сборки
/build
/node_modules

# Игнорировать системные файлы
.DS_Store
*.log
```
Stash (временное сохранение)

```sh
git stash           # Временно сохранить изменения
git stash list      # Показать сохранённые stash
git stash pop       # Вернуть последние сохранённые изменения
```
# 🚀 Продвинутые команды

```sh
git rebase <branch>         # Перебазировать текущую ветку
git cherry-pick <commit>    # Перенести конкретный коммит
git bisect                  # Бинарный поиск бага
git reflog                  # Показать историю всех действий
```
# ❓ Частые проблемы и решения
Проблема: "Your local changes would be overwritten by checkout"


```sh
git stash
git checkout <branch>
git stash pop

Проблема: "Merge conflict"

Откройте файлы с конфликтами

Найдите маркеры <<<<<<<, =======, >>>>>>>

Устраните конфликты

Выполните:
git add <file>
git commit
```


# 📌 Способ 1: Локальная картинка (из репозитория)

```sh
![Альтернативный текст](путь/к/изображению.png)
```
Пример:
```sh
![Логотип Git](images/git-logo.png)
```

# 🌐 Способ 2: Картинка из интернета (по URL)

```sh
![Альтернативный текст](https://example.com/image.jpg)
```
Пример:


```sh
![Git Workflow](https://miro.medium.com/v2/resize:fit:1400/1*diRLm1S5hkVoh5qeArND0Q.png)
```
