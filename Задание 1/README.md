Чтобы создать контейнер нужно скачать с github три файла по ссылке:
git remote add origin https://github.com/Dimasuz/HW_6.4.1.git

затем создать образ:
docker build -t homework-nginx .

запустить контейнер:
docker run --name homework-nginx-container -d -p 7777:80 homework-nginx

и перейти в браузере по ссылке:
localhost:7777