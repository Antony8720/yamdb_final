# yamdb_final
yamdb_final
![example workflow](https://github.com/Antony8720/yamdb_final/actions/workflows/yamdb_workflow.yml/badge.svg)

# Проект: CI и CD проекта api_yamdb

# Автор проекта
**Антон**: https://github.com/Antony8720   

## Описание:

Проект "CI и CD проекта api_yamdb" представляет собой настройку Continuous Integration и Continuous Deployment для приложения api_yamdb: автоматический запуск тестов, обновление образов на Docker Hub, автоматический деплой на боевой сервер при пуше в главную ветку main.

## Процесс развертывания
При пуше в репоизторий в главную ветку main запускаются заранее настроенный workflow: Django-app workflow, включающий в себя

1. job tests
Включает в себя развертывание окружения Python, установку зависимостей, проверку проекта на соответствие PEP8 и запуск, написанных разработчиком тестов

2. job build_and_push_to_docker_hub
Включает в себя пуш образа в Docker Hub

3. job deploy
Включает в себя deploy проекта на боевой сервер

4. job send_message
Включает в себя отправку сообщения в телеграм об успешном выполнении workflow

## Проверка работоспособности:

Для проверки рабосспособности необходимо после выполнения workflow перейти по ссылке:

`http://130.193.55.102`

