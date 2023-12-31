# Авторская база данных с оценкой альбомов

Я являюсь меломаном и в этом проекте решил собрать все прослушанные мной альбомы, которые хотя бы как-то запомнились мне.\
База данных реализована на mySql и стоит на хостинге, но можно использовать плагин json-server для ее симуляции. Сайт стоит локально в моей сети вайфай, потому в нем нет никаких защит и авторизации. (в будущем, возможно, это поменяется).\
Для запросов в базу данных написан бекенд.

## Функционал

1. Отображение списка альбомов с json сервера.
2. Добавление в БД и оценка альбома.
3. Сортировка по некоторым критериям (могут меняться)
4. Поиск конкретного альбома по БД.
5. Оценка альбома по критериям.
6. Просмотр подробной информации об альбоме (В РАЗРАБОТКЕ).
7. Добавление треков к каждому альбому и их последующая оценка (В РАЗРАБОТКЕ).

## Как запустить?

Проект создан с помощью `create-react-app` и запускается следующим образом:
1. Проект клонируется/скачивается.
2. Прописывается `npm init`.
3. Для запуска устанавливаем `json-server`.
4. Запускаем БД: `json-server -p {порт} -w {JSON_файл, у меня в проекте db.json}`.
5. И последнее: `npm start`.

## Скриншоты
### Список всех альбомов
![albums list](https://raw.githubusercontent.com/def1s/rating-albums/719138a/list.png)
### Форма добавления альбома
![add albums form](https://raw.githubusercontent.com/def1s/rating-albums/719138a/add-albums.png)
### Страница отдельного альбома
![single album page without tracks](https://raw.githubusercontent.com/def1s/rating-albums/719138a/without-tracks.png)
### Альбом с добавленными треками
![single album page with tracks](https://raw.githubusercontent.com/def1s/rating-albums/719138a/withtracks.png)