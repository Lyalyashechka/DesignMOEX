# Московская биржа 
## 1. Тема и целевая аудитория.
### 1.1 Тема.
   Московская биржа является крупнейшим организатором торгов акциями, облигациями и другими активами в России. По [данным](https://bcs-express.ru/novosti-i-analitika/top-10-mirovykh-birzh) на июль 2018г. Мос. биржа занимает 22 из 81 место среди крупнейших бирж мира. 
   
   |MVP|
   |---|
   |1. Отслеживание ситуации на рынке| 
   |2. Осуществление сделки на рынке| 
   |3. Получение своей истории торгов на рынке| 
### 1.2 Целевая аудитория.
**По [данным](https://www.moex.com/ru/members.aspx?tid=1179&sby=4) на январь 2022 года количество уникальных клиентов Мос. Биржи:**  
|Тип аудитории      |Кол-во человек|
|-------------------|------------|
|1. Физические лица | 16 779 069 |
|2. Юридические лица | 20 446 |
|3. Иностранные лица | 23 517 |
|4. Иностранные физические лица | 20 685 |
|5. Иностранные юридические лица|  2 832 |
|6. Клиенты, передавшие свои средства в ДУ| 327 432 |
|7. Всего| 17 150 464|  
  
**Основная целевая аудитория** - физические лица, россияне.  
**Портрет российского инвестора согласно сервису** «[Тинькофф инвестиции](https://vc.ru/tinkoff_invest/216367-tinkoff-investicii-sostavili-portret-rossiyskogo-investora-2020)»:  
   |Пол|%|
   |-------|--|
   |Мужчины        |69 %|
   |Женщины        |31 %|  
     
   |Средний возраст|%| 
   |---------------|--|
   |28-38 лет      |43 %|
   |18-28 лет      |27 %|
   |38-48 лет      |21 %|
   |48+            |9  %|  
   
 
## 2. Расчет нагрузки. 
### 2.1 Продуктовые метрики.  
   **2.1.1. Месячная аудитория.**  
   Количество людей, совершивших хотя бы одну сделку в месяц: 2 723 661. [(источник)](https://www.moex.com/ru/members.aspx?tid=1179&sby=4)  

   **2.1.2. Примерная ежедневная аудитория.**  
Торговля на бирже осуществляется с помощью брокеров. Для подсчета ежедневной аудиторией воспользуемся [данными брокера втб](https://www.vtb.ru/o-banke/press-centr/novosti-i-press-relizy/2021/04/2021-04-20-obem-sredstv-pod-upravleniem-vtb-kapital-investitsii-v-i-kvartale-vyros-na-107/#) о количестве уникальных пользователей, ежедневно использующих их мобильное приложение ``` По состоянию на апрель 2021 года - 300 000 человек``` и [данными](https://smart-lab.ru/brokers-rating/russia/stat/) о распределении общего объема пользователей, совершивших хотя бы одну сделку, по брокерам:  
  
![image](https://user-images.githubusercontent.com/77728314/167299298-f57c1b43-4b20-4ede-b8e6-bb2c2746ca67.png)  
  
Предположим, что рост активных пользователей приложения ВТБ был согласно этому графику, тогда с апреля по ноябрь он составил ~30% и ежедневная аудитория составляет ``` 300 000 * 1,3 = 390 000 ```.  
Исходя из графика пользователи ВТБ занимают 14% от общего объема пользователей на мосбирже. Тогда ежедневная аудитория мос.биржи примерно равна ```390 000 / 14 * 100 = 2 785 000``` пользователей.  
  
   **2.1.3. Среднее количество действий пользователя по типам в день**  
   +  **Оформление сделки**  
   Согласно [данным](https://www.moex.com/ru/marketdata/#/mode=groups&group=4&collection=3&boardgroup=57&data_type=history&date=2022-01-19&category=main) среднее количество сделок по парам в январе 2022г. ~3 400 000. Это в примерно 2 раза больше чем на [январь 2021 года](https://www.moex.com/ru/marketdata/#/mode=groups&group=4&collection=3&boardgroup=57&data_type=history&date=2022-01-19&category=main),что соответствует росту количества физических лиц, пользующихся сервисом, в 2 раза за год. Тогда среднее количество сделок на пользователя в день - ```3 400 000/ 2 785 000 = 1,22```
   + **Получение своей истории торгов**  
   Ежедневное количество пользователей биржи 2 785 000, предположим что каждый из них хотя бы раз в среднем сделает запрос на получение 30 своих последних ордеров.  
   + **Получение данных о стакане**  
   Возьмем среднее время сессии пользователя с самой популярной биржи цифровых активов binance.com [00:08:48](https://www.similarweb.com/ru/website/binance.com/#overview) (binance - аналогичный сервис, но торговля в нем происходит без участия брокеров). И предположим что пользователь из этого времени 8 минут наблюдает за стаканом на самом популярном рынке (исходя из данных в п 2.1.3. такой рынок - SBER с 500 000 сделок за торговый день). Сделаем рассчет количества ордеров, информацию о которых пользователя получет за указанное время (при пиковой нагрузке, когда торговля происходит очень быстро, ордер попавший в поле видимости стакана обычного пользователя с большой вероятностью окажется исполненным и превратиться в законченную сделку):  
   ```
 500 000 / 17 / 60 * 8 = 3 921 (17 - количество рабочих часов биржи в сутки)
   ```
   Предположим, что система отправляет запрос на обновление стакана раз в полсекунды, тогда за 8 минут пользователь отправит 960 запросов.  
   |Тип действия | Количество в день| 
   |-------------|------------------|
   |Оформление сделки| 1.22|
   |Получение истории торгов| 1|
   |Отслеживание ситуации в стакане|960|  
   
   **2.1.4. Средний размер хранилища пользователя**   
   Биржа должна хранить информацию о пользователе, осуществляющем торговлю.
   В открытом доступе не удалось узнать какую информацию хранит биржа о пользователе. Но исходя из регистрации сделаем такое предположение:  
   |id пользователя|ФИО|Адрес|Телефон|Адрес электронной почты|Серия и номер паспорта|
   |---------------|---|-----|-------|-----------------------|----------------------|
   |INT            |CHAR(100)|CHAR(300)|(CHAR(14)|CHAR(40)|CHAR(11)|
   |4 байта        |100 байт|300 байт|14 байт|40 байт|11 байт|  
   
   Размер информации о пользователе: ```465 байт```.
   
   Также биржа должна хранить историю торгов одного пользователя.  
Примерный вид одного ордера:  

|id ордера|id пользователя|Пара|Тип ордера (buy или sell)|Тип ордера(LIMIT, MARKET..)|Количество|Время|Цена|Стоп цена|Статус|
|---------|---------------|----|-------------------------|---------------------------|----------|-----|----|---------|------|
|BIGINT      |INT         |INT    |ENUM                  | ENUM                      |FLOAT64   |DATE |FLOAT64|FLOAT64|ENUM|
|8 байт  |4 байта         |4 байта|4 байта               | 4 байта                   | 8 байт  |8 байт|8 байт |8 байт|4 байта|
  
В итоге размер одной сделки в байтах составляет ```60 байт```.

Оценим примерно сколько в среднем сделок хранится у одного пользователя:  
На бирже можно получить историю торгов с 2009 года. Посмотрим на количество пользователей в эти года.  
  
![image](https://user-images.githubusercontent.com/77728314/167309682-30297b57-6744-4b3a-b73f-62fc8c837e88.png)
  
Предположим, что количество пользователей росло пропорционально количеству сделок (подобную закономерность косвенно подтвердили выше).  
Тогда ```16 000 000 / 3 400 000 = 417 000 / x, где x - ежедневное количество сделок, совершаемыми пользователями за 2009 год; x =  142 500```  
Подобным образом вычислим "x" для каждого года, начиная с 2009:  
|2009|2010|2011|2012|2013|2014|2015|2016|2017|2018|2019|2020|2021|
|----|----|----|----|----|----|----|----|----|----|----|----|----|
|142 500|151 700|164 000|171 000|187 000|200 000|214 000|234 000|278 000|415 500|652 000|1 700 000|3 400 000|  

Просуммируем полученные значения и умножим на среднее количество рабочих дней в году(247). 
Общее количество сделок на бирже с 2009 года: ```1 953 695 900```.  

Кроме этого биржа должна хранить информацию о количестве активов у пользователя:  
|id пользователя|id актива|Количество| 
|---------------|---------|----------|
|INT            |INT      |INT       |
|4 байта        |4 байта  |4 байта   |  

По [данным](https://www.tinkoff.ru/about/news/14022020-tinkoff-investments-research-retail-investor-portrait/) Тинькофф инвестиций - в среднем у одного пользователя 11 акций в портфеле.  
Тогда на количество активов пользователя приходится ``` 4 * 3 * 11 = 132 байта ``` 
```
В среднем размер хранилища одного пользователя:  1 953 695 900 / 16 779 069 * 60 байт + 465 байт + 132 байта = ~7,405 Кб.
```

### 2.2 Технические метрики.   
   **2.2.1 Размер хранения в разбивки по типам данных**  
   Информация о пользователях: ```465 байт * 27 657 626 = 12 860 796 090 байт = 11,98 Гб```  ([информация о количестве аккаунтов физ.лиц](https://www.moex.com/ru/members.aspx?tid=1179&sby=4))  
   
   Информация о сделках пользователей: ```60 байт * 1 953 695 900 = 109,17 Гб``` 
   
   Также биржа должна хранить информацию о торгах, для построения графиков.  
   По [данным](https://www.moex.com/ru/listing/securities.aspx) на январь 2022г на бирже торгуется 3625 активов. Биржа постоянно проводит листинг новых бумаг и удаляет другие, однако по данным из этого же источника в 2014 году на бирже торговалось 3675 активов, будем считать что в среднем на бирже торгуется 3650 активов. Также в среднем биржа предоставляет данные по истории торгов начиная с 2008 года. Минимальный масштаб графика - 1 минута. Для отображения линейного графика нужна средняя цена за эту минуту, а для отображения графика "японские свечи" нужна минимальная и максимальная цена за эту минуту. Таким образом можно сделать предположение, что таблица выглядит так:  
   
   |id актива|Дата|Средний прайс|Мин. прайс|Макс. прайс| 
   |---------|----|-------------|----------|-----------|
   |INT      |DATETIME|FLOAT     |FLOAT    |FLOAT      | 
   |4 байта  |8 байт  |8 байт   |8байт     |8 байт     |  
   
   До 20 июня 2020г. торги на бирже проводились с 10:00 до 18:40 по московскому времени, с 20 июня с 10:00 до 23:50, а с 1 марта 2021 с 7:00 до 23:50. Посчитаем какое количество информации хранит биржа об истории торгов активами с 1 января 2009г. по 1 января 2022г:  
   * 01.01.2009 - 20.06.2020: ```(247 * 11 + 110) * 520 * 3650 * 36 байт = 193 163 256 000 байт  (11 - количество лет с 2009 по 2020, 110 количество рабочих дней до 20.06.2020, 520 - количество минут в рабочем дне``` 
   * 20.06.20 - 01.03.2021 ```(137 + 34) * 830 * 3650 * 36 байт = 18 649 602 000 байт```  
   * 01.03.2021 - 01.01.2022 ```213 * 1010 * 3650 * 36 байт = 28 268 082 000 байт```  
  
   Общее количество информации о торгах: ```240 080 940 000 байт = 224,3 Гб```  
   
   **2.2.2. Сетевой трафик**  
   ***2.2.2.1. Пиковое потребление в течении суток***  
   Исходя из котировок биржи основной объем торгов приходится на момент времени с 10:00 до 11:00 (в данный момент в это время происходит открытие торгов):  
   ![image](https://user-images.githubusercontent.com/77728314/167316052-ac4f923a-161e-4b12-9a14-0dbceccba066.png)
  
   Довольно часто на этот период приходится 25 процентов всех дневных торгов, более того в первые 15 минут этого часа совершается 50 процентов объема торгов всего часа. Тогда предположим, что за эти 15 минут может совершаться 12,5 процентов всех дневных сделок на бирже т.е. ```3 400 000 * 0,125 = 425 000``` , учитывая что в среднем один пользователей совершает 1,22 сделки в день, то количество пользователей в этот момент ``` 425 000 / 1,22 = 348 360```.  
   Как уже отмечалось ранее: самый популярный актив на момент января 2021 - акции Сбербанка, если за эти 15 минут совершиться 12,5 процентов сделок по бумаге Сбербанка т.е ```500 000 * 0,125 = 62 500```, то за 1 минуту пребывания на данной паре, пользователь в среднем получит ```62 500 / 15 = 4 166``` сообщения об обновлении стакана. Исходя из изложенного выше максимум нагрузки возможен если все 348 360 пользователей в один момент будут наблюдать за стаканом на паре Сбербанка. Однако, даже если часть пользователей в этот момент будут наблюдать за стаканом на другой паре, то нагрузка уменьшится несущественно. 
    
   Для истории сделок по сети передается следующая информация:  
   
   |Пара|Тип ордера (buy или sell)|Тип ордера(LIMIT, MARKET..)|Количество|Время|Цена|Стоп цена|Статус|
   |----|-------------------------|---------------------------|----------|-----|----|---------|------|
   |СHAR    |ENUM                  | ENUM                      |FLOAT64   |DATE |FLOAT64|FLOAT64|ENUM|
   |16 байт|4 байта               | 4 байта                   | 8 байт  |8 байт|8 байт |8 байт|4 байта|  
   
   Всего: 60 байт. 
   
   Для отображения одного ордера в стакане по сети передается следующая информация:  
   
   |Тип ордера (buy или sell)|Количество|Цена|
   |-------------------------|----------|----|
   |ENUM                     |FLOAT64   |FLOAT64|
   |4 байта                  | 8 байт  |8 байт |  
   
   Всего: 20 байт.
   
   Для оформление сделки по сети передается следующая информация:  
   
   |Пара|Тип ордера (buy или sell)|Тип ордера(LIMIT, MARKET..)|Количество|Цена|Стоп цена|
   |----|-------------------------|---------------------------|----------|----|---------|
   |INT    |ENUM                  | ENUM                      |FLOAT64   |FLOAT64|FLOAT64|
   |4 байта|4 байта               | 4 байта                   | 8 байт  |8 байт |8 байт|  
   
   Всего: 36 байт. 
   ```
   Пиковый трафик по просмотру истории своих сделок: 348 360 * 60 байт * 30 = 627 048 000 байт/15мин = 680,39 Кб/с;
   (30 - количество ордеров, о которых получаем информацию)  
   Пиковый трафик по просмотру текущих сделок в стакане: 348 360 * 4 166 * 20 байт / 60 с  = 3,7 Гбит/с  
   Пиковый трафик по оформлению сделок: 425 000 / 15 / 60 * 36 байт = 17 000 байт/с = 16,6Кб/с 
```  
```
Максимальная нагрузка примерно равна 3,7 Гбит/с, остальными показателями можно пренебречь,  
с учетом того что все пользователи не могут одновременно наблюдать за стаканом и просматривать историю своих сделок.  
(при оформлении сделки возможно продолжать наблюдать за стаканом)
```
   ***2.2.2.2. Суммарный суточный*** 
   ```Суточный трафик по просмотру истории своих сделок: 2 785 000 * 30 * 60 байт = 4,67 ГБ/сутки  
      Суточный трафик по просмотру текущих ордеров в стакане: 2 785 000 * 3921 * 20 байт = 203,4 ГБ/сутки  
      Суточный трафик по оформлению сделок: 2 785 000 * 1,22 * 36 байт = 0,11 ГБ/сутки  
   ```  
   **2.2.3. RPS в разбивке по типам запросов**  
   * Количество запросов в сутки на получение истории своей торговли: 2 785 000.  
   * Количество запросов в сутки на получение данных из стакана:      2 785 000 * 960 = 2 673 600 000.  
   * Количество запросов в сутки на оформление сделок:                2 785 000 * 1,22 = 3 397 700.  
   
   Для получения RPS делим эти данные на (17 * 60 * 60).  
      
   |Тип запроса | RPS|
   |------------|----|
   |Получение истории своей торговли| 45,5|
   |Получение данных из стакана     | 61 200|
   |Оформление сделки               | 55,51|  
      
   RPS при пиковом трафике для получения данных из стакана:  ```348 360 * 2 = 696 720 (2 - количество запросов от одного пользователя в секунду)```  
## 3. Логическая схема. 
![Highload_3 (2)](https://user-images.githubusercontent.com/77728314/167402429-82fcc976-d67b-4186-9a11-b1954b81d265.jpg)
## 4. Физическая схема.  
  ![hihgload_physic](https://user-images.githubusercontent.com/77728314/167424213-763c4a04-1299-4c24-a45e-427ade0485cf.jpg)

  4.1. Индексы. 
  orders - индексы по user_id; (trade_pare_id, time)  
  trade_history - индекс (id_trade_pare, time)  
  4.2. Шардирование. 
  Как отмечалось выше на бирже торгуется 3650 ценных бумаг. Таблицу с временными рядами и таблицу orders можно шардировать по id_trade_pare. Таким образом мы существенно ускорим получение истории торговли и списка сделок.  
  Виртуальные шарды будем мапить на сервера по следующему принципу:  
  На бирже все активы делятся на 3 уровня по доверенности биржи к этим активам. Подавляющий объем торгов приходится на активы 1 уровня, таких активов 776, их будем мапить по 8 виртуальных шардов на 1 физический сервер. Оставшиеся 3 000 будем мапить по 100 на один физ. сервер.  
## 5. Технологии.  
|Технология|Область применения|Мотивационная часть| 
|----------|------------------|-------------------|
|PostgreSql|Таблицы пользователей, активов, торговых пар| Данный сегмент данных не подвержен частым изменениям, в качестве базы данных было выбрано наиболее популярное и развитое решение среди открытых СУБД. Также возможность хранить в postgreSQL объекты может быть очень полезна для хранения специфических данных об активе или пользователе.| 
|InfluxDB|Таблица с временными рядами торговых пар| Influx новое решение с открытым исходным кодом, специализирующееся на хранение временных рядов. Оно имеет высокую пропускную способность для поступающих данных, позволяет выполнять сжатие и запрашивать эти же самые данные в реальном времени. InfluxDB была разработана с самого начала, с целью обеспечить высокомасштабируемый механизм приема и хранения данных. Он очень эффективен при сборе, хранении, запросе, визуализации и выполнении действий с потоками данных временных рядов, событий и метрик в реальном времени.|  
|MemSQL|Таблицы ордеров, активов пользователя| MemSQL позиционирует себе как новый класс БД HTAP (Hybrid transactional / analytical processing). MemSQL обходит узкое место ввода-вывода большинства алтернативных БД, помещая данные в память и переводя SQL на C++, что позволяет базе данных отправлять больше транзакций в секунду с чрезвычайно низкой задержкой (<1 мс на запрос). MemSQL совместим с MySQL и для работы с ним можно использовать те же инструменты и драйверы, что и для MySQL. Также одним из преимуществ MemSQL является предоставление аналитики в режиме реального времени.|  
|JAVA|Основной ЯП системы|На данный момент JAVA это баланс между временем на разработку, качеством, вычислительной точностью и скоростью работы. На JAVE написано огромное количество коммерческих программ, в том числе с высокой нагрузкой. Регулярные обновления, возможность сохранения обратной совместимости между версиями и многолетняя положительная репутация позволяют выбрать JAVA в качестве основного ЯП.|  
## 6. Схема проекта. 
![Untitled Diagram (9)](https://user-images.githubusercontent.com/77728314/167515689-eefe8afe-bc1d-4a38-8e74-9c8175db8abb.jpg)

На NGINX будет осуществляться L7 балансировка между серверами.  
Используем Nginx для балансировки нагрузки и в качестве reverse-proxy. В качестве алгоритма балансировки будем использовать round-robin так как он обеспечивает в среднем равномерную балансировку для неблокирующих соедениний.  

Сам проект состоит из 3 микросервисов:  
* *history_api* отвечает за отдачу пользователям временных рядов истории торговли.  
* *simple_data_api* отвечает за регистрацию новых пользователей, просмотр и добавление торговых пар и активов.  
* *trade_api* отвечает за оформление и просмотр ордеров на рынках.  

После создания или обновления ордера в MemSQL бд происходит перерасчет значений в Influx бд.  

## 7. Список серверов.
* NGINX   
В среднем NGINX выдает 300 RPS на 1 ядро.  
Возьмем 64 ядерные процессоры, тогда при пиковой нагрузке нам необходимо ```696 720 / (300 * 64) = 37 ``` серверов.  
* trade_api  
Самый нагруженный сервер. Исходя из собственных тестов на 4 ядерном процессоре java spring сервер способен выдавать 2700 rps (запросы с 1 походом в базу данных), исходя из этих данных предположим, что 64 ядерный процессор способен выдавать 43 200 rps, тогда при пиковой нагрузке нам нужно ```696 720 / 43 200 = 16``` таких серверов.  
* history_api  
Нагрузка на этот сервер существенно ниже чем на trade_api. Предположим, что в пике 348 360 пользователей будут смотреть график истории торгов одновременно, посылая запрос на получение данных о следующей порции временных рядов раз в 2 секунды, тогда количество RPS = 174 180. Количество серверов ```174 180 / 43 200 = 4``` 
* simple_data_api  
Самый ненагруженный сервер, предположим, что в пике на него будет приходится 80 000 RPS, тогда нам понадобится ```2``` сервера.  
* InflexDB  
Исходя из пункта 4.2 нам понадобится ``` 800 / 8 + 3 000 / 100 = 130``` серверов. Размер истории торгов для 1 пары достаточно маленький и нам с запасом хватит 64Гб RAM и SSD на 64Гб для каждого из них.  
* MemSQL  
Нам также понадобится 130 серверов и нам также с запасом хватит 64Гб RAM и SSD на 64Гб.  
* PostgreSQL  
Хранит информацию о ~30 000 000 млн пользователей и 4 000 активах и парах. Это примерно ```30 000 000 * 465 байт + 8 000 * 200 байт = ~15Гб```. Хватит 1 сервера

Все сервера для api и балансировки будем брать x2 с запасом по мощности, и x2 для сервером БД для реплик.  
|Сервис	|CPU (ядер)|	RAM (ГБ)	|Диск(Гб	|Количество|  
|--------|----------|------------|-----|----------|  
|NGINX   |64        |64          |SSD 64|37 + 37 |
|trade_api|64        |64         |SSD 64|16 + 16  |
|history_api|64      |64         |SSD 64|4 + 4     |
|simple_data_api|64| 64          |SSD 64|2 + 2| 
|InflexDB        |32|64          |SSD 64|130 +130 |
|MemSQL          |32|64          |SSD 64|130 +130 |
|PostgreSQL      |32|64          |SSD 64|1 + 1|  

## Источники информации. 
1. https://bcs-express.ru/novosti-i-analitika/top-10-mirovykh-birzh
2. https://www.moex.com/ru/members.aspx?tid=1179&sby=4
3. https://vc.ru/tinkoff_invest/216367-tinkoff-investicii-sostavili-portret-rossiyskogo-investora-2020
4. https://www.vtb.ru/o-banke/press-centr/novosti-i-press-relizy/2021/04/2021-04-20-obem-sredstv-pod-upravleniem-vtb-kapital-investitsii-v-i-kvartale-vyros-na-107/#
5. https://smart-lab.ru/brokers-rating/russia/stat/
6. https://www.moex.com/ru/marketdata/#/mode=groups&group=4&collection=3&boardgroup=57&data_type=history&date=2022-01-19&category=main
7. https://www.similarweb.com/ru/website/binance.com/#overview 
8. https://www.tinkoff.ru/about/news/14022020-tinkoff-investments-research-retail-investor-portrait/
