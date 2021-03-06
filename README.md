# Imagespark

## Посмотреть проект онлайн можно по ссылке **[https://nakkutricks.github.io/image-spark/](https://nakkutricks.github.io/image-spark/)**

## ❓📃 Задача:
Реализовать поиск пользователей **[github](https://github.com/)** используя **[github api](https://docs.github.com/en/rest)** <br />

## ❗📃 Требования и результат:
- Поиск: по логину | :heavy_check_mark:
- Сортировка: по количеству репозиториев (возрастанию/убыванию) | :heavy_check_mark:
- Подгрузка списка при скролле, либо пагинация | :heavy_check_mark:
- При клике на элемент - открываются подробности (как и какие на усмотрение разработчика) | :heavy_check_mark:
- Для работы с данными использовать Vuex | :heavy_check_mark:
- Для навигации - VueRouter | :heavy_check_mark:

## :white_check_mark: Дополнительно:
- Список пользователей и карточка пользователя отображаются через localStorage, поэтому при перезагрузке страницы данные остаются на месте.
- Сделан адаптив под мобильные устройства и планшет.
- Добавлена небольшая интерактивность в виде анимаций.
- Попытался реализовать дизайн в стиле сайта imagespark.

## :hammer_and_wrench: Что из задуманного мной реализовать не удалось:
- Планировал сделать бесконечную подгрузку пользователей, но быстро реализовать логику без костылей не получилось, поэтому пришлось делать классическую пагинацию.
- В карточке пользователя хотел выводить список репозиториев, но понял, что в этом нет необходимости, так как подобную логику я реализовал в списке пользователей. К тому же для этого пришлось бы делать дополнительные запросы на сервер, а на них установлен лимит.
- Хотел увеличить количество запросов на сервер, но, к сожалению, разобраться смог только с токеном пользователя, который, конечно, я использовать не стал.

## 🧙 Как можно улучшить:
- При загрузке карточки пользователя происходит небольшой пролаг, тк ответ от сервера приходит не сразу. На такой случай можно добавить заглушку-лоадер, а пользователя показывать при полной загрузке с сервера.
- Написать корректные проверки ошибок. Сейчас проверка работает по типу - если есть ошибка (не важно какая), сделать то-то. Нужно персонализировать ошибки.
- Для визуального отображения ошибок стилизовать отдельные блоки. Сейчас реализовано через alert.
- Можно еще нормальные коммиты начать писать.

## 🧰 Используемые инструменты при разработке

### Логика:
- Vue 2
- Vue-router
- Vuex

### Верстка:
- HTML5
- CSS3
- БЭМ
- Sass

## 💻 Запустить проект локально

##### 1. `npm i` – установить зависимости проекта

##### 2. `npm run serve` – запуск приложения
