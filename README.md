# Point 1<br/>
* забрать файлы из репозитория GitHub [здесь](https://github.com/JunAndrey/Docker/tree/main/point_1)<br/>
* создать образ:<br/>
  docker build . -t <имя образа><br/>
* запустить образ:<br/>
  docker run -d -p 7777:80 -v <абсолютный путь до директории с вашим html-файлом>:/usr/share/nginx/html --name <имя контейнера> <имя образа><br/>
  Флаг -v и последующие пути используются для замены дефолтной nginx-страницы на ваш html-файл<br/> 
  для Win -v C:\\Users\\<путь до директории>:/usr/share/nginx/html<br/>
  для Linux -v /home/<и т.д.>:/usr/share/nginx/html<br/>
  в качестве html-файла можно использовать [это](https://github.com/JunAndrey/Docker/blob/main/point_1/index.html)<br/>

# Point 2<br/>
* Вы можете:<br/>
* забрать файлы из репозитория GitHub [здесь](https://github.com/JunAndrey/Docker/tree/main/point_2)<br/>
* создать образ:<br/>
  docker build . -t <имя образа><br/>
* запустить образ:<br/>
  docker run -d -p 7777:6060 --name <имя контейнера> <имя образа><br/>
