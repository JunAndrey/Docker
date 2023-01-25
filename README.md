## Point 1<br/>
* забрать файлы из репозитория GitHub [здесь](https://github.com/JunAndrey/Docker/tree/main/point_1)<br/>
* создать образ:<br/>
  `docker build . -t <имя образа>`<br/>
* запустить образ:<br/>
  `docker run -d -p 7777:80 -v <абсолютный путь до директории с вашим html-файлом>:/usr/share/nginx/html --name <имя контейнера> <имя образа>`<br/>
  Флаг -v и последующие пути используются для замены дефолтной nginx-страницы на ваш html-файл, путём подмены директории html<br/> 
  для ***Win***   `-v C:\\Users\\<путь до директории>\\html:/usr/share/nginx/html`<br/>
  для ***Linux***   `-v /home/<и т.д.>/html:/usr/share/nginx/html`<br/>
  в качестве html-файла можно использовать [это](https://github.com/JunAndrey/Docker/blob/main/point_1/index.html)<br/>
* проверить результат командой `curl localhost:7777`

## Point 2<br/>
* Вы можете:<br/>
* забрать файлы из репозитория GitHub [здесь](https://github.com/JunAndrey/Docker/tree/main/point_2)<br/>
* создать образ:<br/>
  `docker build . -t <имя образа>`<br/>
* запустить образ:<br/>
  `docker run -d -p 8000:6060 --name <имя контейнера> <имя образа>`<br/>
* проверить результат командой `curl localhost:8000`
* после отображения страницы в url добавить `/api/v1/`
  например `http://127.0.0.1:8000/api/v1/`
