<img src="https://github.com/DenisChervony/web-images/blob/main/YandexPrilavok.png" alt="Denis Chervony" align="center" style="width:100%; height:auto;">

# Новая функциональность в API Яндекс.Прилавка

Разработчики сделали новую функциональность в API Яндекс.Прилавка. Новую версию API передали тебе на тестирование. 

<details>
  <summary>Ссылки для работы:</summary> 
  
- Тестовый стенд: [https://{id}.serverhub.praktikum-services.ru/](https://{id}.serverhub.praktikum-services.ru/)
- Документация API: [https://{id}.serverhub.praktikum-services.ru/docs/](https://{id}.serverhub.praktikum-services.ru/docs/)
- [Требования к бэкенду](https://code.s3.yandex.net/qa/files/backend_requirements.pdf)
  
 </details> 

 <details>
   <summary>Задача</summary>
  
### Предусловия ###

**Работа с наборами:** возможность добавлять продукты в набор — ручка `POST /api/v1/kits/{id}/products`.

**Работа с курьерами:** возможность проверить, есть ли доставка курьерской службой «Привезём быстро» и сколько она стоит. 
Ручка `POST /fast-delivery/v3.1.1/calculate-delivery.xml`. 

**Работа с корзиной:** 
- возможность получить список продуктов,  которые добавили в корзину. Ручка `GET /api/v1/orders/id`;
- возможность добавлять продукты в корзину. Ручка `PUT /api/v1/orders/:id`;
- возможность удалять корзину. Ручка `DELETE/api/v1/orders/:id`.

### Постановка задачи ###
- Проанализируй требования к новой функциональности бэкенда Яндекс.Прилавка. Изучи документацию к API в Apidoc. Требования к бэкенду находятся [здесь](https://code.s3.yandex.net/qa/files/backend_requirements.pdf).
- Спроектируй тесты в виде чек-листа, чтобы покрыть функциональность, которую тебе передали на тестирование: она описана выше. Авторизацию проверять не нужно.
- Протестируй API через Postman и заведи баг-репорты в Google Таблицу, если это понадобится.

 </details> 


 <details>
  <summary>Чек-листы и Баг-репорты</summary>

 [Чек-листы и Баг-репорты, ссылка на докемент](https://docs.google.com/spreadsheets/d/1Y3vnKlT3PDjsaYkxcgJ_pLwlawlEAwJJbat9BNtxkkU/edit?usp=sharing)

  </details>
 
 <details>
  <summary>Отчёт о тестировании</summary>

  [Отчёт о тестировании, ссылка на докемент](https://docs.google.com/document/d/1gpl_Xx5YgNa9D8BnXjO003FFYcKc2DOcitlFGRdEM3A/edit?usp=sharing)
 
 
 # Отчет о тестировании Яндекс.Метро
 
Тестирование проводилось в следующем тестовом окружении: 
- Эмулятор: Android Studio, 
- Устройство: Honor 8, 
- ОС: Android 9.0 Pie - API 28, 
- Разрешение экрана: 1080х1920, 
- Диагональ: 5,5,
- Версия Яндекс.Метро: 3.6.



Все требования, затронутые изменениями, были покрыты чек-листом [ссылка на Google-таблицу](https://docs.google.com/spreadsheets/d/1Y3vnKlT3PDjsaYkxcgJ_pLwlawlEAwJJbat9BNtxkkU/edit?usp=sharing). 

Также написан регрессионный чек-лист: [ссылка на Google-таблицу](https://docs.google.com/spreadsheets/d/1Y3vnKlT3PDjsaYkxcgJ_pLwlawlEAwJJbat9BNtxkkU/edit?usp=sharing). 

Результаты выполнения тестов можно посмотреть здесь: [ссылка на Google-таблицу](https://docs.google.com/spreadsheets/d/1Y3vnKlT3PDjsaYkxcgJ_pLwlawlEAwJJbat9BNtxkkU/edit?usp=sharing). 


Из 56 успешно прошло 46, не прошло — 10.

 
 ## Список багов, найденных при тестировании, разбит по приоритетам:
 
 ### 1. Блокирующие: 
 *Не найдено*
 
 ### 2. Критичные:
 - [Временной интервал маршрута не обновляется при превышении текущим временем времени окончания](https://docs.google.com/spreadsheets/d/1Y3vnKlT3PDjsaYkxcgJ_pLwlawlEAwJJbat9BNtxkkU/edit?gid=589506703#gid=589506703&range=A5)
 - [При нажатии на кнопку "Обратная связь" происходит переход в приложении Googl почты](https://docs.google.com/spreadsheets/d/1Y3vnKlT3PDjsaYkxcgJ_pLwlawlEAwJJbat9BNtxkkU/edit?gid=589506703#gid=589506703&range=A11)
 - [Карта не масштабируется жестами "Пинч" и "Спред"](https://docs.google.com/spreadsheets/d/1Y3vnKlT3PDjsaYkxcgJ_pLwlawlEAwJJbat9BNtxkkU/edit?gid=589506703#gid=589506703&range=A13)
 
 ### 3. Средний приоритет:
 - [Новые станции появляются в низу списка в истории.](https://docs.google.com/spreadsheets/d/1Y3vnKlT3PDjsaYkxcgJ_pLwlawlEAwJJbat9BNtxkkU/edit?gid=589506703#gid=589506703&range=A4)
 - [При смене ориентации экрана масштаб построенного маршрута не сохраняется в том состоянии, которое выбрал пользователь.](https://docs.google.com/spreadsheets/d/1Y3vnKlT3PDjsaYkxcgJ_pLwlawlEAwJJbat9BNtxkkU/edit?gid=589506703#gid=589506703&range=A6)
 - [При переходе из портретной ориентации в альбомную и обратно, карточка Маршрута свёрнутое меняется на среднее положение.](https://docs.google.com/spreadsheets/d/1Y3vnKlT3PDjsaYkxcgJ_pLwlawlEAwJJbat9BNtxkkU/edit?gid=589506703#gid=589506703&range=A7)
 - [При переходе из портретной ориентации в альбомную, карточка Станции из среднего положения переходит в свернутое.](https://docs.google.com/spreadsheets/d/1Y3vnKlT3PDjsaYkxcgJ_pLwlawlEAwJJbat9BNtxkkU/edit?gid=589506703#gid=589506703&range=A8)
 - [При переходе из портретной ориентации в альбомную, карточка Станции из открытого положения переходит в среднее.](https://docs.google.com/spreadsheets/d/1Y3vnKlT3PDjsaYkxcgJ_pLwlawlEAwJJbat9BNtxkkU/edit?gid=589506703#gid=589506703&range=A9)
 - [При отсутствии интернет-соединения уведомление об ошибке не появляется.](https://docs.google.com/spreadsheets/d/1Y3vnKlT3PDjsaYkxcgJ_pLwlawlEAwJJbat9BNtxkkU/edit?gid=589506703#gid=589506703&range=A10)
 - [В режиме "Автоматически" тема в 18:00 не меняется на темную.](https://docs.google.com/spreadsheets/d/1Y3vnKlT3PDjsaYkxcgJ_pLwlawlEAwJJbat9BNtxkkU/edit?gid=589506703#gid=589506703&range=A12)
 
 ### 4. Низкий приоритет:
 *Не найдено*
 
 ### 5. Незначительные:
*Не найдено*
 
 ### Примечание:
 С учётом того, что блокирующие ошибки не обнаружены, однако выявлены критические дефекты, способный дезориентировать пользователей, а также несколько серьезных багов, которые могут негативно повлиять на впечатление от работы с приложением, команда тестирования рекомендует выпустить обновление в Google Play исключительно после устранения указанных недостатков.  

 
 ## Тестирование производительности заняло 6 часов  
Не все найденные дефекты критически влияют на взаимодействие с приложением. Основные пользовательские сценарии (построение маршрута, просмотр станций) остаются доступными. Однако критические баги, такие как некорректное отображение временных интервалов и проблемы с масштабированием карты, могут дезориентировать и негативно повлиять на опыт пользователей.  

После исправления багов я бы порекомендовал:  
- Провести повторное тестирование критических дефектов (временные интервалы, масштабирование карты, работа с ориентацией экрана).    
- Проверить смену темы приложения в автоматическом режиме на разных устройствах.  
- Выполнить тестирование на реальных устройствах (для выявления проблем, которые могли не проявиться на эмуляторе).  
- Обработать сценарии отсутствия интернета.
- Доработать обработку смены ориентации экрана 


 </details>
