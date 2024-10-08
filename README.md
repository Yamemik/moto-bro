# Moto-BRO (backend)

![Static Badge](https://img.shields.io/badge/Yamemik-moto_bro-moto_bro)
![GitHub top language](https://img.shields.io/github/languages/top/Yamemik/moto-bro)
![GitHub](https://img.shields.io/github/license/Yamemik/moto-bro)
![GitHub Repo stars](https://img.shields.io/github/stars/Yamemik/noto-bro)
![GitHub issues](https://img.shields.io/github/issues/Yamemik/moto-bro)


## Общее описание
_____
### Стек технологий:
  - FastAPI;
  - postgreSQL;
  - docker;
  - docker-compose.


## Техническое описание
_____

### инструмент для управления зависимостями Poetry
```bash
# установить poetry на Windows
$ (Invoke-WebRequest -Uri https://install.python-poetry.org -UseBasicParsing).Content | py -
# на Mac or Linux system
$ curl -sSL https://install.python-poetry.org | python3 -
# создавать виртуальное окружение virtualenvs в корневом каталоге проекта
$ poetry config virtualenvs.in-project true
# инициализировать Poetry-проект
$ poetry init
# добавление пакетов
$ poetry add fastapi uvicorn
$ poetry add sqlalchemy
```

### команды MakeFile
```bash
# запустить контейнер с приложением
$ make app
```

### fastapi
```bash
# запустить сервер
$ uvicorn --factory src.main:create_app --reload
```

### docker & docker-compose
```bash
# собрать
$ docker compose -f docker_compose/app.yaml up
# ребилдинг
$ docker build --no-cache -t docker_compose-fastapi .
```


## Ссылки
_____
[by Yamemik](https://github.com/Yamemik)