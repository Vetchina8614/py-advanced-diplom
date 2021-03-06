# Дипломная работа


## VKinder
Все слышали про известное приложение для знакомств - Tinder. Приложение предоставляет простой интерфейс для выбора понравившегося человека. Сейчас в Google Play у Tinder более 100 миллионов установок.

## Задание
Используя данные из VK нужно сделать сервис намного лучше чем Tinder. Сервис должен искать людей, подходящих под условия, на основании информации о пользователе из VK:
- диапазон возраста,
- пол,
- группы,
- расположение,
- интересы,
- любой другой необязательный параметр.

У каждого критерия поиска должны быть свои приоритеты. Например, совпадение по возрасту важнее общих групп, интересы по музыке важнее книг, наличие общих друзей важнее возраста.

Разбор похожих интересов — книги, музыка и т.д. нужно будет провести с помощью анализа текста.

У тех людей, которые подошли по требованиям, собирать по три самые популярные фотографии с аватара. Популярность определяется по количеству лайков.

## Входные данные
Имя пользователя или его id в VK, для которого мы ищем пару. Если информации недостаточно, нужно дополнительно спросить её у пользователя.


## Выходные данные
JSON-файл с 10 объектами, где у каждого объекта перечислены три его самые популярные фотографии и ссылка на аккаунт.

## Обязательные требования к сервису:
1. Код программы удовлетворяет`PEP8`.
2. Сервис может получать токен от пользователя с нужными правами.
3. Программа декомпозирована на функции/классы/модули/пакеты.
4. Результат сервис записывает в БД.
5. Результаты не должны повторяться при повторном поиске.
6. Сервис проходит базовое функциональное тестирование.
7. Не запрещается использовать внешние библиотеки для vk.


## Дополнительные требования:
1. В VK максимальная выдача при поиске 1000 человек. Подумайте, как это ограничение можно обойти.
2. Возможность ставить/убирать лайк выбранной фотографии.
3. Добавлять человека в избранный список, используя БД.
4. Добавлять человека в чёрный список, чтобы он больше не попадался в выдаче, используя БД.
5. К списку фотографий из аватарок добавлять список фотографий, где отмечен пользователь.
