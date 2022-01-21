[![CI](https://github.com/kotsenkom/yamdb_final/actions/workflows/yamdb_workflow.yml/badge.svg?branch=master)](https://github.com/kotsenkom/yamdb_final/actions/workflows/yamdb_workflow.yml)
# yamdb_final
yamdb_final
## Описание проекта

Командный учебный проект написанный в рамках обучения в Яндекс.Практикум.

На основе архитетуры REST API был реализован проект YaMDb, позволяющий пользователям оставлять отзывы на произведения. Произведения делятся на категории: "Книги", "Фильмы", "Музыка". Список категорий может быть расширен пользователем с ролью администратор. В каждой категории есть произведения: книги, фильмы или музыка. Произведения можно присваивать жанр из предустановленных. Новые жанры могут создавать админитраторы. Обычные пользователи могут отправлять текстовые отзывы к произведениям и ставить оценку в диапазоне от одного до десяти. Из пользовательских оценок формируется усредненная оценка произведения - рейтинг. На одно произведение пользователь может ставить только один отзыв.

## Запуск проекта
1. Клонировать репозиторий с github

git clone https://github.com/KotsenkoM/yamdb_final.git

2. Перейти в каталог infra

cd yamdb_final/api_yamdb/infra

3. Запустить Dockerfile 

sudo docker-compose up -d --build


Проект доступен по url http://localhost/

## Инфраструктура проекта
Для работы с проектом необходимо добавить переменные в .env

DB_ENGINE=<django.db.backends.postgresql>
DB_NAME=<имя базы данных postgres>
DB_USER=<пользователь бд>
DB_PASSWORD=<пароль>
DB_HOST=<db>
DB_PORT=<5432>
SECRET_KEY=<секретный ключ проекта django>

## Автор
Максим Коценко https://github.com/KotsenkoM/yamdb_final