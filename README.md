Если новый проект:

1 Создаем в корне папку ./src

2 Переходим в ./src - и с консоли запускаем: 
    docker compose run composer create-project laravel/laravel .

3 Возвращаемся в корень и в консоле: docker compose build

4 Дальше в консоле: docker compose up

5 Если пишет ошибку laravel.log, то переходим в контейнер php и меняем права на папку ./storage
    chown -R www-data:www-data storage
    
    
    
Если стянули проект:

1 В консоле: docker compose build

2 Дальше в консоле: docker compose up

Если пишет 500 ошибка - добавьте .env в ./src