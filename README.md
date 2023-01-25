Point 1
забрать файлы из репозитория GitHub
создать образ:
docker build . -t <имя образа>
запустить образ:
docker run -d -p 7777:80 -v <абсолютный путь до директории с вашим html-файлом>:/usr/share/nginx/html --name <имя контейнера> <имя образа>
Флаг -v и последующие пути используются для замены дефолтной nginx-страницы на ваш html-файл 
для Win -v C:\\Users\\<путь до директории>:/usr/share/nginx/html
для Linux -v /home/<и т.д.>:/usr/share/nginx/html
в качестве html-файла можно использовать это-https://github.com/JunAndrey/Docker/blob/main/point_1/index.html
Point 2
Вы можете:
забрать файлы из репозитория GitHub
создать образ:
docker build . -t <имя образа>
запустить образ:
docker run -d -p 7777:6060 --name <имя контейнера> <имя образа>
