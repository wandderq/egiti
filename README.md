# egiti
egiti (Easy GIT Ignore) - это утилита для быстрого управления gitignore-файлами в проекте. egiti использует GitHub API для получения макетов gitignore (см. [REST API endpoints for gitignore](https://docs.github.com/en/rest/gitignore/gitignore?apiVersion=2026-03-10&versionId=free-pro-team%40latest&productId=rest))

## Возможности
- Создание новых gitignore файлов: `egiti init --templates Python`
- Создание и удаление новых записей: `egiti add .venv .python-version`
- Скачивание готовых макетов .gitignore: `egiti load C Cmake`
- Просмотр записей в файле: `egiti show --comments`

Все возможности утилиты можно просмотреть используя `egiti --help`

## Установка
1. Через pip/pipx
    ```bash
    pipx install egiti
    ```
    или с github (последняя версия, может быть нестабильна)
    ```bash
    pipx install git+https://github.com/wandderq/egiti@main
    ```

2. Из исходного кода
    ```bash
    git clone https://github.com/wandderq/egiti@main
    cd egiti
    pip install -e .
    ```


## Лицензия
Эта утилита распространяется под [MIT лицензией](https://github.com/wandderq/egiti/blob/main/LICENSE)