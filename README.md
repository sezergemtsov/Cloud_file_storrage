## Проект "Облачное хранилище"

### Общая информация

Проект облачного хранилища представляет собой web приложение позволяющее загружать, хранить и скачивать файлы.
Фронтенд для приложения написан не мной, а взят [здесь](https://github.com/netology-code/jd-homeworks/tree/master/diploma/netology-diplom-frontend)  
Бэкэнд реализован на Java как REST приложения на основе Spring framework.  
В данном репозитории для упращения установки использован jar файл. Полную информацию о серверной части проекта с подробным описанием можно найти
[здесь](https://github.com/sezergemtsov/REST-api-on-docker/blob/master/docker-compose.yaml)  

### Запуск и настройка

Проект собран с помощью Docker, поэтому едиственное что должно быть установлено на хосте на момент запуска непосредственно сам Docker.

Для запуска необходимо скачать репозиторий в удобное место, открыть в терминале путь к нему и запустить командой "docker compose up"

По умолчанию приложение запустится на http://localhost:8081

Для правильной конфигурации следует проверить свободны ли следующие порты:  
Фронт использует 8081, бэкэнд использует 8085, база данных использует 8087.  
Для изменения следует изменить только первое значение в [docker-compose.yaml](https://github.com/sezergemtsov/Cloud_file_storrage/blob/master/docker-compose.yaml)  
как на изображении ниже:  
![alt text](https://github.com/sezergemtsov/Cloud_file_storrage/blob/master/port.png)
 
