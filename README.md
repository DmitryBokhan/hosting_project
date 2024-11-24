https://www.youtube.com/watch?v=SX-f0n4fdYI&list=PLd2_Os8Cj3t9Ert8mBlNl1UqwllyP1Tm_&index=13

#### Список запущенных контейнеров
- docker ps

#### Проверить логи 
- docker logs <container_id>

### Перезагрузка контейнера 
- docker-compose restart [*имя контейнера*]
- пример:  docker-compose restart db

#### Поднять/опустить контейнер
- docker-compose down
- docker-compose up -d

- docker-compose -f docker-compose.yml up -d --build  (для локалки)
- docker-compose -f docker-compose.dev.yml up -d --build  (для Production)

- docker-compose up -d --build  (пересобрать контейнер)

#### Зайти в контейнер
- sudo docker exec -it [*имя контейнера*] bash 
- пример: sudo docker exec -it project_app bash  

#### Открыть права на все файлы в папке
sudo chmod 777 -R ./

- docker logs project_app 
- docker ps



## CI/CD GitHib

Переменные:
- https://docs.github.com/ru/actions/writing-workflows/choosing-what-your-workflow-does/store-information-in-variables
- https://www.youtube.com/watch?v=zn5T7FkpaTA 


## github runner

Устанавливаем на нашу VM


./run.sh
