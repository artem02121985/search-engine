# search-engine

Приложение для быстрого поиска страниц, содержащих текстовый запрос.
Поиск проводиться по индексированным сайтам, список которых устанавлевает пользователь.
Запуск индексации осуществляется пользователем.
В меню доступны следующие действия:
  - "DASHBOARD" просмотр статистики. Результаты статистики можно увидеть после обновления страницы.  
  - "MANAGEMENT" запуск и остановка индексации. После остановки индексации появляется поле "add/update" где можно добавить или обновить страницу.
  Доменное имя страницы должно соответствовать одному из имен сайтов установленного списка. Так-же можно запустить индексацию заново. Если сайт был
  проиндексирован и в момент переиндексации недоступен, старые данные сохраняються.
   
  - "SEARCH" позволяет сделать запрос по всем либо по одному сайту из списка. Результаты поиска пявляються после отправленного запроса.


## В приложении использовались следующие технологии:
  
  - Framework Spring 
  - ForkJoinPool
  - база данных MySQL
  - лемматизация apache lucene
  - Jsoup
  - JPA
  - Apache Tom Cat
  - HikkariPool
  - JDBC

## Установка и запуск приложения.
  - Клонируем ссылку на репозиторий.
  
  - Открываем проект в среде разработки, например IntellejIdea,в правом верхнем углу, кликаем по "Maven", выбираем "LifeCicle" 
    и кликаем
 "package". В папке "target" появиться файл.jar
  - В конфигурационном файле "application.yaml" устанавливаем данные порта для нашего приложения и данные подключения к базе  "user", "password" и путь к MySQL серверу. Так же указываем данные сайта "url" и "name". Сайтов может быть несколько.
  ![forReadme](https://user-images.githubusercontent.com/95944672/235514432-ecaa7da2-6e07-4a0c-802d-b4f58eb3991d.png)
  
  - Открываем командную строку и запускаем .jar файл
  
  ## Возможные проблемы с запуском
  -Для запуска используйте ту же версию Java которая, компилировала архив. Это может быть Java используемая вашей средой разработки.
  
  
