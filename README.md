# Тестирование страницы https://gost-group.ru/en/

### Открывается главная страница:
<img src = "https://github.com/Suburbanknight89/GOST-group_tests/blob/master/src/test/resources/img/Main%20page.png">

### Параметры (по умолчанию) для запуска через Jenkins:

* browser (default chrome)
* browserVersion (default 89.0)
* browserSize (default 1920x1080)
* browserMobileView (mobile device name, for example iPhone X)
* remoteDriverUrl (selenoid.autotests.cloud)
* videoStorage (url address where you should get video)
* threads (number of threads)

### Интсрукция для запуска тестов через Jenkins:
  <img src = "https://github.com/Suburbanknight89/GOST-group_tests/blob/master/src/test/resources/img/jenkins_sborka.png">


Run tests with filled remote.properties:
```bash
gradle clean test
```

Run tests with not filled remote.properties:
```bash
gradle clean -DremoteDriverUrl=https://user1:1234@selenoid.autotests.cloud/wd/hub/ -DvideoStorage=https://selenoid.autotests.cloud/video/ -Dthreads=1 test
```

Serve report:
```bash
allure serve build/allure-results
```


For further development there are some example tests in src/test/java/cloud.autotests/tests/demowebshop
* remove @Disabled("...") annotation to run tests
```bash
gradle clean demowebshop
```

:heart: <a target="_blank" href="https://qa.guru">qa.guru</a><br/>
:blue_heart: <a target="_blank" href="https://t.me/qa_automation">t.me/qa_automation</a>


