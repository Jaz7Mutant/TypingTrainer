# Typing Trainer Game
Версия: 1.1
Автор: Даниил JazzMutant Толстоухов (d-a-ny4@ya.ru)

## Описание
Клавиатурный тренажер, в форме игры. Поддерживает игру по сети.

##
Допы: 
* Разные режимы игры
* Игра по сети
* Звуки

## Состав
* Сама игра `TypingTrainer.py`
* Модули `typingtrainer/` 
* Тесты `tests/`
* Словари `dictionaries/`

Справка: `python TypingTrainer.py --help`

Запуск игры: `python TypingTrainer.py`

## Режимы игры
* Common texts
* Random words (только в одиночной игре)
* Python code

## Сетевая игра
Для игры по сети необходимо создать комнату с необходимыми настройками, дождаться подключения других игроков и запустить игру. После завершения раунда всем игрокам приходит таблица результатов.

## Подробности реализации
Все модули игры находятся в папке `typetrainer`. Модуль `game` отвечает за проведение раунда, то есть взаимодействия с пользователем. Модули `*_menu` реализуют визуализацию и интерфейс. `socket_client` содержит в себе инструментарий для сетевой игры.
Класс `Game` формирует статистику или же количество очков, в зависимости от режима игры.
Тексты формируются классом `TextGenerator` 

Тесты можно найти в папке `tests`

    typetrainer\game.py                  95     18    81%
    typetrainer\texts_generator.py       34      6    82%
