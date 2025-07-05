# Ruff linter template
Шаблон для использования статического анализатора python кода

# Target project usage
Для интеграции шаблона в целевой проект необходимо:

```yaml
# Добавление шаблона 
include:
  - project: 'skillbox-michlew/linter-template'
    file: 'linter.yml'
# Первая стадия с линтером
stages:
- linter
...
# Активация шаблона
linter:
  extends: .lint-ruff
```