# Тестирование страницы https://gost-group.ru/en/
<img src = "https://github.com/Suburbanknight89/GOST-group_tests/blob/master/src/test/resources/img/Main%20page.png">


### Список автоматизированных и ручных тестов в AlluretestOps:
<img src = "https://github.com/Suburbanknight89/GOST-group_tests/blob/master/src/test/resources/img/testOpstests.png">

### Параметры (по умолчанию) для запуска через Jenkins:

* browser (default chrome)
* browserVersion (default 89.0)
* browserSize (default 1920x1080)
* browserMobileView (mobile device name, for example iPhone X)
* remoteDriverUrl (selenoid.autotests.cloud)
* videoStorage (url address where you should get video)
* threads (number of threads)

### Инструкция для запуска тестов через [Jenkins](https://jenkins.autotests.cloud/job/GOST-group_tests.git/):

  <img src = "https://github.com/Suburbanknight89/GOST-group_tests/blob/master/src/test/resources/img/jenkins_sborka.png">


### Запуск тестов с заполненными local.properties (команда в терминале Idea):
```bash
gradle clean test
```

### Удаленный запуск тестов (команда в терминале Idea):
```bash
gradle clean -DremoteDriverUrl=https://user1:1234@selenoid.autotests.cloud/wd/hub/ -DvideoStorage=https://selenoid.autotests.cloud/video/ -Dthreads=1 test
```

### Allure отчет (команда в терминале Idea):
```bash
allure serve build/allure-results
```
### Анализ прохождения тестов в Allure-report:
<img src = "https://github.com/Suburbanknight89/GOST-group_tests/blob/master/src/test/resources/img/allureseults.png">

### Оповещение об окончании прогона тестов в телеграмм:
<img src = "https://github.com/Suburbanknight89/GOST-group_tests/blob/master/src/test/resources/img/telegram.JPG">

## Видео прохождения теста "3 Успешный поиск тура", взятое из среды выполнения (из Selenoid)
<img src = "https://github.com/Suburbanknight89/GOST-group_tests/blob/master/src/test/resources/img/telegram.JPG">

:heart: <a target="_blank" href="https://qa.guru">qa.guru</a><br/>
:blue_heart: <a target="_blank" href="https://t.me/qa_automation">t.me/qa_automation</a>


