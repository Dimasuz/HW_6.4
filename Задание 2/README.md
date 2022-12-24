Чтобы создать контейнер нужно скачать с github три файла по ссылке:
git remote add origin https://github.com/Dimasuz/HW_6.4.1.git

затем создать образ:
docker build -t homework-add .

запустить контейнер:
docker run --name homework-container -d -p 8000:8000 homework-add

и перейти в браузере по ссылке:
http://127.0.0.1:8000/