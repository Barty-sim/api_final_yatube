### Описание проекта
**Это API создан для взаимодействия с прошлым проектом Yatube и построен на его базе**
### Как запустить проект:
Клонировать репозиторий и перейти в него в командной строке:
```
https://github.com/Barty-sim/api_final_yatube
```
```
cd api_final_yatube
```
Cоздать и активировать виртуальное окружение:
```
python -m venv venv
```
```
. venv/Scripts/activate
```
```
python -m pip install --upgrade pip
```
Установить зависимости из файла requirements.txt:
```
pip install -r requirements.txt
```
Выполнить миграции:
```
python manage.py migrate
```
Запустить проект:
```
python manage.py runserver
```
### После запуска
**После запуска проекта, по адресу http://127.0.0.1:8000/redoc/ документация для API Yatube, с описанием как должен работать проект.
### Примеры
**Для доступа к API необходимо получить токен: 
Нужно выполнить POST-запрос localhost:8000/api/v1/token/ передав поля username и password. API вернет JWT-токен**
**Дальше, передав токен можно будет обращаться к методам, например: **
**/api/v1/posts/ (GET, POST, PUT, PATCH, DELETE)**
**При отправке запроса передавайте токен в заголовке Authorization: Bearer <токен>**