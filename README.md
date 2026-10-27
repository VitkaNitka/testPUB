*Док для проекта testPUBproject*
# Как создать Git-репозиторий и загрузить его на GitHub

### 1. Создать папку проекта и перейти в неё

```bash
mkdir my-project
cd my-project
```

### 2. Инициализировать Git-репозиторий

```bash
git init
```

### 3. Создать файлы проекта

Например, создать `README.md` и добавить в него описание проекта.

### 4. Добавить файлы в staging area

```bash
git add --all
```

### 5. Создать коммит

```bash
git commit -m "Initial commit"
```

### 6. Создать репозиторий на GitHub

- Открыть GitHub и нажать **New repository**.
- Указать название репозитория.
- Выбрать Public или Private.
- Не добавлять README, `.gitignore` и лицензию, если они уже есть локально.
- Нажать **Create repository**.

### 7. Связать локальный репозиторий с GitHub через SSH

Скопировать SSH-адрес репозитория на GitHub и выполнить:

```bash
git remote add origin git@github.com:USERNAME/REPOSITORY.git
```

### 8. Проверить подключение

```bash
git remote -v
```

### 9. Отправить коммит на GitHub

Проверить название текущей ветки:

```bash
git branch --show-current
```

Отправить ветку (если она называется `main`):

```bash
git push -u origin main
```

Если ветка называется `master`, использовать `master` вместо `main`.

---

## Как отправлять последующие изменения

После редактирования файлов:

```bash
git add --all
git commit -m "Describe changes"
git push
```

**Полезные команды:**

- `git status` — проверить состояние файлов.
- `git remote -v` — проверить адрес удалённого репозитория.
- `git log --oneline` — посмотреть историю коммитов.