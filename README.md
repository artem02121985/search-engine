# search-engine

Приложение для быстрого поиска страниц.
Поиск проводиться по индексированным сайтам, список которых устанавлевает пользователь.
Запуск индексации осуществляется пользователем.Запрос состоит из текста, который есть на странице.
В меню доступны следующие действия:
  - "DASHBOARD" просмотр статистики. Результаты статистики можно увидеть после обновления страницы.  
  - "MANAGEMENT" запуск и остановка индексации. После остановки индексации появляется поле "add/update" где можно добавить или обновить страницу.
  Доменное имя страницы должно соответствовать одному из имен сайтов установленного списка. Так-же можно запустить индексацию заново. Если сайт был
  проиндексирован и в момент переиндексации недоступен, старые данные сохраняються.
   
  - "SEARCH" позволяет сделать запрос по всем либо по одному сайту из списка. Результаты поиска пявляються после отправки запроса.


## В приложении использовались следующие технологии:
  
- Framework Spring Boot
  - JPA
  - Apache Tom Cat
  - HikkariPool
  - Hibernate
- ForkJoinPool
- лемматизация apache lucene
- Jsoup
- mysql-connector-java
- projectlombok
 

## Установка и запуск приложения.
- Клонируем ссылку на репозиторий.
- Открываем проект в среде разработки, например IntelliJIdea.
- В конфигурационном файле "application.yaml" устанавливаем:
  - данные порта для этого приложения. 
  - данные подключения к базе данных  datasource: "user", "password" и "url" путь к MySQL серверу.
  - Так же указываем данные сайтов sites: "url" и "name".
  - При необходимости можно поменять свойства "connection-settings".


Скриншот файла application.yaml с настройками

![Снимок экрана (108)](https://github.com/artem02121985/search-engine/assets/95944672/a78836cf-6e5c-47a6-8694-7381b91ab334)


- в правом верхнем углу, кликаем по "Maven", выбираем "LifeCicle" 
    и кликаем
 "package". В папке "target" появиться файл.jar, как в скриншоте.

- Открываем командную строку и запускаем файл.jar
- Меню управления откроется в браузере устройства по http://localhost/
  
  ## Возможные проблемы с запуском
- Для запуска используйте ту же версию Java в которой создавался архив.
  
  
  
