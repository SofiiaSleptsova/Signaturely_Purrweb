# <a name="up" />Проект Signaturely

О проекте: Signaturely - это веб-сервис, предназначенный для удобной и безопасной электронной подписи документов. Сервис предоставляет пользователям возможность создавать, редактировать и подписывать различные типы документов онлайн, без необходимости использования бумажных копий или ручных подписей.

## Содержание
- [Задачи тестировщика](#задачи-тестировщика)
- [Объект тестирования](#объект-тестирования)
- [Инструменты](#инструменты)
- [Планирование тестирования](#планирование-тестирования)
- [Проектирование тестовой документации](#проектирование-тестовой-документации)
- [Баг-репорты](#баг-репорты)
  
## Задачи тестировщика

<details>
<summary> Задачи </summary> 

1. Изучить сайт Signaturely;
2. Подробно описать стратегию (план) тестирования (что, как и когда проверять);
3. Добавить чек-лист проверок для страницы /documents;
4. Добавить к документу 3 баг-репорта.

***

</details>

## Объект тестирования

Сайт https://signaturely.com

## Инструменты
<p align="left"> 
  <a href="https://docs.google.com/" target="_blank" rel="noreferrer"><img src="https://w7.pngwing.com/pngs/240/1015/png-transparent-g-suite-google-docs-google-angle-rectangle-logo.png" width="36" height="36" alt="Google Sheets" /></a>
  <a href="https://www.jetbrains.com/youtrack/" target="_blank" rel="noreferrer"><img src="https://upload.wikimedia.org/wikipedia/commons/9/95/YouTrack_Icon.png" width="36" height="36" alt="Youtrack" /></a>
   <a href="https://miro.com/" target="_blank" rel="noreferrer"><img src="https://w7.pngwing.com/pngs/885/629/png-transparent-miro-hd-logo-thumbnail.png" width="36" height="36" alt="Miro" /></a>
</p> 

## Планирование тестирования

### Тест-анализ сервиса
**Декомпозиция и визуализация сервиса Signaturely**
![iScreen Shoter - Safari - 231108152918](https://github.com/SofiiaSleptsova/Signaturely/assets/147629405/57695b70-3a88-4d25-8e47-944c1cc9c453)

### Мастер-план тестирования проекта
Тестирование состоит из семи этапов.  
Временная шкала по итерациям: Длительность каждого этапа может варьироваться, но общий план нацелен на завершение тестирования в течение 2-3 месяцев.  
Команда тестирования: QA-инженер Слепцов София.   
Тестовая среда: Тестирование будет проводиться в тестовой среде, отделенной от продуктивной среды.  
Риски: Потенциальные риски включают недостаточное время для тестирования, неожиданные технические сложности и изменения в требованиях.  

**Этап 1: Функциональное тестирование**    
Описание: Проверка основных функций сервиса, включая создание, редактирование и подписание документов, а также функции авторизации и регистрации.  
Цели: Гарантировать, что пользователи могут успешно взаимодействовать с функциональностью сервиса, входить в свои аккаунты и регистрироваться.  
Принципы: Тестировать сценарии использования, соответствие требованиям и удовлетворение потребностей пользователей.  
Что тестировать: Вход в систему, выход из системы, регистрация новых пользователей, восстановление пароля, функции создания, редактирования и подписания документов.  
Что не тестировать: Интеграцию.  
Критерии входа: Завершенная разработка основных функций сервиса, включая авторизацию и регистрацию.  
Критерии выхода: Успешное прохождение всех функциональных тестов, включая авторизацию и регистрацию.  

**Этап 2: Интеграционное тестирование**  
Описание: Проверка взаимодействия Signaturely с облачными хранилищами данных, такими как Google Drive, Box, One Drive и Dropbox, и информационной страницы о сайте.  
Цели: Убедиться, что интеграция с облачными хранилищами работает корректно, и информационная страница отображается правильно.  
Принципы: Тестировать сценарии загрузки и синхронизации документов, а также правильность отображения информации на информационной странице.  
Что тестировать: Интеграцию с облачными хранилищами, передачу данных между ними, и отображение информации на информационной странице.  
Что не тестировать: Безопасность и производительность на данном этапе.  
Критерии входа: Завершенная интеграция с хранилищами данных и создание информационной страницы.  
Критерии выхода: Успешное интеграционное тестирование и правильное отображение информации на странице.  

**Этап 3: Тестирование безопасности**  
Описание: Проверка мер безопасности, включая шифрование данных при передаче и сохранение конфиденциальной информации.  
Цели: Гарантировать, что пользовательские данные и документы хранятся и передаются безопасно, и информационная страница не содержит уязвимостей.  
Принципы: Тестировать шифрование, безопасность авторизации, защиту от взлома, и анализ информационной страницы на предмет уязвимостей.  
Что тестировать: Защиту данных, безопасность авторизации, обработку ошибок, и анализ информационной страницы.  
Что не тестировать: Функциональность и производительность.  
Критерии входа: Завершенная реализация мер безопасности и информационной страницы.  
Критерии выхода: Успешное прохождение всех тестов безопасности и отсутствие уязвимостей на информационной странице.  

**Этап 4: Производительность и нагрузочное тестирование**  
Описание: Оценка производительности сервиса, времени загрузки страниц, и его поведения при больших объемах данных и пользователей.  
Цели: Гарантировать, что сервис работает быстро и стабильно даже при больших нагрузках.  
Принципы: Тестировать время загрузки страниц, производительность функций, и стабильность при больших объемах данных и пользователей.  
Что тестировать: Скорость загрузки страниц, обработку документов, и поведение системы при больших нагрузках.  
Что не тестировать: Функциональность и безопасность на данном этапе.  
Критерии входа: Завершение функционального, безопасносного и информационного тестирования.  
Критерии выхода: Успешное прохождение тестов производительности и нагрузки, а также корректное отображение информационной страницы.  

**Этап 5: Тестирование удобства использования и кроссбраузерное тестирование, а также проверка на различных устройствах**  
Описание: Этот этап оценивает интерфейс и удобство использования Signaturely, а также обеспечивает совместимость сайта с разными браузерами, устройствами и их разрешениями.  
Цели: Гарантировать, что пользователи могут легко и комфортно использовать Signaturely на различных устройствах, в том числе на десктопах, ноутбуках, планшетах и мобильных устройствах.  
Принципы: Тестирование дизайна, навигации, интуитивности использования и обеспечение совместимости с различными устройствами.  
Что тестировать: Дизайн интерфейса, навигацию, интуитивность использования на разных устройствах и разрешениях экрана. При кроссбраузерном тестировании также проверяется совместимость с разными браузерами.  
Что не тестировать: Технические аспекты и безопасность, которые тестировались на предыдущих этапах.  
Критерии входа: Завершение разработки интерфейса и адаптивного дизайна.  
Критерии выхода: Успешное прохождение тестов удобства использования на различных устройствах и совместимость с разными браузерами.  

**Этап 6: Регрессионное тестирование**  
Описание: Повторное тестирование после внесения изменений и исправления дефектов, а также проверка информационной страницы после изменений.  
Цели: Убедиться, что исправления не повлияли на работоспособность других функций и что информационная страница корректно отображается после изменений.  
Принципы: Тестировать сценарии использования после изменений и проверять информационную страницу на предмет изменений.  
Что тестировать: Все основные функции сервиса, а также информационную страницу.  
Что не тестировать: Интеграцию и производительность.  
Критерии входа: Внесение изменений или исправлений.  
Критерии выхода: Успешное прохождение регрессионных тестов и корректное отображение информационной страницы после изменений.  

**Этап 7: Финальное тестирование и подготовка к релизу**  
Описание: Финальное тестирование всей функциональности и подготовка к выпуску сервиса, а также проверка информационной страницы перед релизом.  
Цели: Гарантировать готовность сервиса к публичному доступу и корректное отображение информационной страницы.  
Принципы: Проверка всех аспектов функциональности и безопасности, а также информационной страницы.  
Что тестировать: Все функции и аспекты сервиса, а также информационную страницу.  
Что не тестировать: Внутренние технические детали.  
Критерии входа: Завершение всех предыдущих этапов тестирования и информационной страницы.  
Критерии выхода: Готовность сервиса к релизу и информационной страницы без ошибок и уязвимостей.  

#### Тест-анализ вкладки
**Декомпозиция и визуализация вкладки Documents (по функциональности)**

![iScreen Shoter - Safari - 231108153641](https://github.com/SofiiaSleptsova/Signaturely/assets/147629405/f7167d67-fb75-4f54-bc49-3717d45da4fe)

### Детальный план тестирования вкладки "Documents"  
**Стратегия:**    
Применима стратегия по ручному тестированию, указанным видам тестирования  

**Приоритет:**     
Приоритет тестирования высокий для всех видов тестирования, так как раздел "Documents" является ключевой функциональностью сервиса. Однако, следуя оптимальному порядку тестирования, предлагается следующий приоритет:     
-Смоук-тестирование  
-Функциональное тестирование  
-Тестирование пользовательского интерфейса  
-Кроссплатформенное тестирование  
-Тестирование удобства использования  
Такой порядок позволит сначала проверить базовую работоспособность, а затем провести более подробное тестирование.

**Виды тестирования:**    
1. Смоук тестирование:  
Провести смоук тестирование, чтобы убедиться, что основные функции работают;  
2. Функциональное тестирование:  
Параметры поиска;  
Отображения полученных и отправленных документов;  
Корректная работа дополнительных опций с документом;  
3. Тестирование удобства использования:  
Оценка дизайна и навигации в разделе "Documents"  
4. Тестирование пользовательского интерфейса  
Проверить все ли элементы расположены корректно  
+Кроссплатформенное тестирование
 
**Критерии начала тестирования:**  
Веб-сервис Signaturely находится в активной разработке.  
Все основные функции вкладки "Documents" (создание, редактирование, подписание документов) реализованы и доступны для тестирования.  
Базовый функционал вкладки "Documents" прошел успешное смоук-тестирование и функциональное тестирование.  

**Критерии окончания тестирования:**    
Все задачи тестировщика, включая выполнение чек-листов и тест-кейсов, завершены.  
Найденные дефекты зарегистрированы в баг-репортах с указанием описания, приоритета и статуса.  
Все дефекты, обнаруженные в ходе тестирования, пройдены процессом верификации и решены.  
Тестировщик составил отчет о тестировании, включая общий результат и рекомендации для улучшения качества вкладки "Documents".  
Вся тестовая документация (чек-листы, тест-кейсы, баг-репорты) актуальна и подготовлена к передаче разработчикам и менеджерам проекта.  
Все задачи по тестированию удовлетворяют установленным критериям качества и приняты заказчиком или менеджером проекта.  

**Техники тест-дизайна:**  
-Эквивалентное разделение;  
-Граничное значение;  
-Парные комбинации.  

**Тестовая документация:**  
-Чек-листы;  
-Тест-кейсы;  
-Баг-репорты;  
-Отчет о тестировании.  

**Окружение:**  
Операционные системы:   
-Windows;  
-macOS;   
-Linux;  
-Android;  
-IOS;  
Браузеры:  
-Google Chrome;  
-Mozilla Firefox;  
-Microsoft Edge;  
-Safari;  
-Opera;  
-Internet Explorer (если необходима поддержка устаревших версий).  

## Проектирование тестовой документации

![Чек-лист](https://github.com/SofiiaSleptsova/Signaturely/assets/147629405/975a0d79-3b13-4d62-ae98-20ae45c0a3f4)

*тестирование по чек-листу не проходило

## Баг-репорты

<details>
<summary> ID: SIGN-1 </summary> 

### Option Share: В попапе Share this Document прокрутка наверх становится невозможным при добавлении более 8 зрителей [SIGN-1](https://slepsovasonya.youtrack.cloud/issue/SIGN-1/Option-Share-V-popape-Share-this-Document-prokrutka-naverh-stanovitsya-nevozmozhnym-pri-dobavlenii-bolee-8-zritelej)

**Предусловия:**  
1. Открыть сайт https://staging.d2twwklgqmrfet.amplifyapp.com/  
2. Зарегистрироваться как пользователь на сайте  
3. Войти в личный кабинет пользователя  
4. Отправить на подпись документ через вкладку Sign  
5. Получатель должен подписать документ через вкладку Documents, тег Received  
6. Нажать на вкладку Documents  

**Шаги воспроизведения:**  
1. У документа со статусом Completed нажать на кнопку Option на странице Documents  
2. Нажать на кнопку Share из раскрывающего списка Option  
3. В поле ввода test@signaturely.com вести валидный почтовый адрес в попапе Share this Document  
4. Нажать на поле Add Viewer в попапе Share this Document  
5. Повторить шаг 3 и 4 более 8 раз  

**Ожидаемый результат:**   
При добавлении более 8 зрителей в попапе Share this Documents, прокрутка наверх возможна   
**Фактический результат:**  
При добавлении более 8 зрителей в попапе Share this Document, прокрутка наверх становится невозможным  
[видео](https://slepsovasonya.youtrack.cloud/api/files/8-164?sign=MTY5OTY2MDgwMDAwMHwxLTF8OC0xNjR8ZzVMWmI0THJva0R6aUE0VWNCc2RJb0JJNzk1NU5lSzFxbUk5V0d0dlBXaw0K&updated=1698639665490)

**Приоритет:**   
Серьезная             

**Окружение:**  
MacOS  
Браузер: воспроизводится везде  
***
</details>

<details>
<summary> ID: SIGN-2 </summary> 

### Create Folder: папка не появляется в блоке документов, созданная через страницу Documents тег - Received [SIGN-2](https://slepsovasonya.youtrack.cloud/issue/SIGN-2/Create-Folder-papka-ne-poyavlyaetsya-v-bloke-dokumentov-sozdannaya-cherez-stranicu-Documents-teg-Received)

**Предусловия:**  
1. Открыть сайт https://staging.d2twwklgqmrfet.amplifyapp.com/  
2. Зарегистрироваться как пользователь на сайте  
3. Войти в личный кабинет пользователя  
4. Нажать на вкладку Documents   

**Шаги воспроизведения:**  
1. Нажать на тег Received на вкладке Documents  
2. Нажать на кнопку Create Folder на страниц Documents  
3. Нажать поле New Folder Name в попапе Create Folder  
4. В поле New Folder Name ввести название папки  
5. Нажать на кнопку Create в попапе Create Folder  

**Ожидаемый результат:**   
Папка появляется в блоке документов, созданная на странице Documents Received  
**Фактический результат:**    
Папка НЕ появляется в блоке документов, созданная на странице Documents Received (можно посмотреть только через опцию Move to+нет возможности удалить созданные папки)  
[видео](https://slepsovasonya.youtrack.cloud/api/files/8-166?sign=MTY5OTY2MDgwMDAwMHwxLTF8OC0xNjZ8c1BaY1l0YW9EQ1RGb0NJNlE1b1ZacUlCdkF3enlkam8yU3ctbEJoTWhoSQ0K&updated=1698641311619)

**Приоритет:**   
Серьезная             

**Окружение:**  
MacOS  
Браузер: воспроизводится везде  
***
</details>

<details>
<summary> ID: SIGN-3 </summary> 

### Option Generate Singing Link: Сгенерированная ссылка открывается и подписание возможно инициатором документа [SIGN-3](https://slepsovasonya.youtrack.cloud/issue/SIGN-3/Option-Generate-Singing-Link-Sgenerirovannaya-ssylka-otkryvaetsya-i-podpisanie-vozmozhno-iniciatorom-dokumenta)

**Предусловия:**  
1. Открыть сайт https://staging.d2twwklgqmrfet.amplifyapp.com/  
2. Зарегистрироваться как пользователь на сайте  
3. Войти в личный кабинет пользователя  
4. Нажать на вкладку Sign  
5. Отправить документ на подписание  

**Шаги воспроизведения:**  
1. Нажать на вкладку Documents  
2. Нажать Option у документа со статусом Awaiting  
3. Нажать опцию Generate Singing Link  
4. В попапе Generate Singing Link нажать на кнопку Get Singing Link  
5. В браузере открыть новую вкладку и вставить ссылку из буфера, нажать Enter  
6. В открывшейся странице-на странице подписания нажать на место заполнения  
7. В попапе Choose Signature выбрать подпись  
8. В попапе Choose Signature нажать на кнопку Sign Now  
9. На странице подписания нажать на кнопку Send  
10. В попапе Almost done нажать на кнопку I agree  

**Ожидаемый результат:**  
Сгенерированная ссылка открывается и подписание возможно только получателем/ями  
**Фактический результат:**  
Сгенерированная ссылка открывается и подписание возможно инициатором документа  

**Приоритет:**   
Критическая             

**Окружение:**  
MacOS  
Браузер: воспроизводится везде  

***
</details>
