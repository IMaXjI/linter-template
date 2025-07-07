# Ruff linter template
Шаблон для использования статического анализатора python кода

# Target project usage
Для интеграции шаблона в целевой проект необходимо:

```yaml
# Создать job с вызовом reusable workflow из целевого проекта  
jobs:
  linter:
    uses: IMaXjI/linter-template/.github/workflows/linter.yml@main
  # Добавить зависимость от линтера на последующие стадии
  next_job:
    ...
    needs: linter
```