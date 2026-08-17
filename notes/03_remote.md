# Удаленные репозитории

## git remote
Управление удаленными репозиториями

```bash
git remote -v                    # Показывает все удаленные репозитории
git remote add origin URL        # Добавляет удаленный репозиторий
git remote remove origin         # Удаляет связь с удаленным репозиторием
```

## git clone
Копирует удаленный репозиторий к себе на компьютер

```bash
git clone https://github.com/user/repo.git
```

## git push
Отправляет изменения в удаленный репозиторий

```bash
git push origin master           # Отправляет ветку master в origin
git push -u origin master        # Отправляет и запоминает связь
```

## git pull
Забирает изменения из удаленного репозитория

```bash
git pull origin master           # Забирает изменения и сливает
git fetch                        # Просто забирает, но не сливает
```

## git remote show
Показывает подробную информацию об удаленном репозитории

```bash
git remote show origin
```

### Важно!
1. Сначала создаешь репозиторий на GitHub
2. Затем привязываешь его к локальному: `git remote add origin URL`
3. И только потом делаешь первый `git push -u origin master`