
# Ветвление и слияние

## git branch
Управление ветками

```bash
git branch                 # Показывает список всех веток
git branch new-branch      # Создает новую ветку
git branch -d branch-name  # Удаляет ветку
git branch -m old new      # Переименовывает ветку
```

## git checkout
Переключение между ветками

```bash
git checkout branch-name   # Переключается на существующую ветку
git checkout -b new-branch # Создает и переключается на новую ветку
```

## git switch (новая команда)
Альтернатива checkout для переключения

```bash
git switch branch-name     # Переключается на ветку
git switch -c new-branch   # Создает и переключается
```

## git merge
Слияние веток

```bash
git merge branch-name      # Вливает branch-name в текущую ветку
```

### Важно!
Перед слиянием всегда проверяй, что ты находишься в той ветке, КУДА хочешь влить изменения:
```bash
git status                 # Покажет, где ты находишься
git checkout main          # Переключился на главную ветку
git merge feature-branch   # Влил фичу в главную
```