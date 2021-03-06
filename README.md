# Ivorlun microservices repository


[![Build Status](https://travis-ci.org/Otus-DevOps-2018-02/Ivorlun_microservices.svg?branch=master)](https://travis-ci.org/Otus-DevOps-2018-02/Ivorlun_microservices)
____

## Docker 1

* Установлена экоситема docker
* Изучены основные команды работы с docker
* Освоена некоторая часть основ докер-системы

### Задание со *

#### Образ от контейнера отличается наличием

* информации для публикации в репозиторий - тэгами, автором образа, датой создавния и т.п.
* хэш суммами слоёв образа - для проверки наличия изменений при пересборке
* параметрами конфигурации ОС, создаваемой из образа - архитектурой, переменными, пользователями, томами и тп.

#### Контейнер от образа отличается наличием

* текущего статуса конетейнера и соответсвующими параметрами - статусом(запущен ли), номер процесса на хосте и т.п.
* хэш суммой родительского __образа__ контейнера из которого он создан
* различной текущей конфигурацией - куда пишет на хост логи, куда файлы, имя
* настройками виртуального железа и сети

#### Что общего - конфигурация контейнера

Итого - образ и контейнер разные сущности.
Образ - это шаблон для создания контейнеров. Из одного неизменного образа можно создать множество контейнеров.
Контейнер - это облегчённая псевдовиртуальная машина, которая при запуске воссаздаёт окружение описанное в образе,
после чего может быть модифицированна в процессе работы на хост системе.
____