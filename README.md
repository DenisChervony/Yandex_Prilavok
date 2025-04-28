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

 [Чек-листы и Баг-репорты, ссылка на докемент](https://docs.google.com/spreadsheets/d/113hOZr9NLbMTYB6e9SK_Gd01myN7B9vhSyJJlhfx5TY/edit?usp=sharing)

  </details>
 
 <details>
  <summary>Отчёт о тестировании</summary>

  [Отчёт о тестировании, ссылка на докемент](hhttps://docs.google.com/document/d/1N5KHynS9xbwPRxGJUKHN-e6Oe9xJuQBkvNH9UgYkSCA/edit?usp=sharing)
 
 
 # Отчет о тестировании Яндекс.Прилавок
 
Тестирование проводилось в следующем тестовом окружении: 
- Тестовый стенд: https://{id}.serverhub.praktikum-services.ru/
- Документация API: https://{id}.serverhub.praktikum-services.ru/docs/
- Версия Яндекс.ПриЛавок: 3.1.1
- Версия Postman: 11.36.1

 
 ## Тестирование производительности заняло 15 часов  
На данный момент продукт не соответствует критериям релиза: 50% чек-листа содержит критические и блокирующие ошибки (всего 31 баг: 21 критический и 10 блокирующих).
Перед выпуском необходимо исправить все дефекты в текущей API-версии и провести полный ретест!


 </details>
