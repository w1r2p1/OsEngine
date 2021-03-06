# OsEngine

![oslogo250](https://cloud.githubusercontent.com/assets/26077466/23395381/5545b688-fd9f-11e6-8db9-c8e8944a8cc2.png)

# Архитектура [OsEngine] & автоматизации торговли на бирже.
https://drive.google.com/drive/folders/1FA7I1rVR9tt-RobxoRGPnM7gPgNIhlsy

# Архитектура [Voltdb]  хранение данных в памяти с концепцией распределенной 
https://drive.google.com/drive/folders/1YqYZIwWFvy1lP1NMOxrhZrMX7xZj-628

СУБД VoltDB 3.0, развиваемой под руководством Майкла Стоунбрейкера (Mike Stonebraker), одного из основателей проектов Ingres и PostgreSQL. СУБД VoltDB поддерживает горизонтальное масштабирование и ориентирована на обработку транзакций в реальном времени (OLTP). На недорогом кластере, собранном своими силами из обычных серверов, СУБД способна обрабатывать миллионы транзакций в секунду.

# Apache Hadoop Big Data with VoltDB
![Image alt](https://www.voltdb.com/wp-content/uploads/2017/03/Apache-Hadoop-Big-Data-VoltDB.gif)

Идея VoltDB заключается в том, что все транзакции выполняются с помощью предварительно скомпилированных хранимых процедур, реализованных на Java, и все хранимые процедуры сериализуются, что позволяет VoltDB достичь самого высокого уровня изоляции и устранения блокировок. Использование устройства очень хорошее. В официальных результатах испытаний VoltDB может легко масштабироваться до 39 серверов (300 ядер), 120 разделов, обрабатывающих 1,6 миллиона сложных транзакций в секунду.

# Архитектура [Geode] Реверс инжениринг движка обработки финансовых транзакций в торговых платформах различных компаний на Уолл-стрит.
Geode был создан компанией Gemstone Systems в 2002 году и применяется в качестве высокопроизводительного движка обработки финансовых транзакций в торговых платформах различных компаний на Уолл-стрит.

В качестве примера внедрения Geode это Национальная железная дорога Китая, в которой кластер из 20 узлов (10 основных и 10 запасных) обеспечивает хранение 2 Тб оперативной информации о билетах. 
![Image alt](http://chinalogist.ru/sites/default/files/speed-railwas-of-china4.png)

Архитектура [Geode] & Реверс инжениринг движка обработки финансовых транзакций
https://drive.google.com/drive/folders/1tetUejh8WzscoCbCHPsdILM6desm5GzX

# Open Source Algo Trading Platform

[Сайт разработчиков](http://o-s-a.net)

Ну и поскольку она для СНГ и пишется исключительно с русскими комментариями, далее всё на великом...

## Что такое OsEngine?

Это полный комплекс программ необходимых для автоматизации торговли на бирже. 

![default](https://user-images.githubusercontent.com/26077466/42362896-01b3e74a-80fe-11e8-8f36-3db24cb7522c.png)

В него входят:

*Os.Data* - программа для загрузки исторических данных, с помощью которой Вы можете получать свечи, стаканы и тики из самых различных источников.

*Os.Optimizer* - программа для тестирования на истории одной стратегии с разными параметрами.

*Os.Tester* - программа для тестирования на истории множества стратегий одновременно, но без перебора параметров. Поддерживает трансляцию нескольких таймфреймов и нескольких инструментов одновременно.

*Os.Miner* - программа для поиска прибыльных формаций на графике. Как в ручном, так и в автоматическом режиме. Работа с БигДатой у Вас на компьютере. Паттерны найденные при помощи этой программы можно запускать в торговлю.

*Os.Trader* - программа для торговли на бирже. 

Слой создания роботов у нас работает как с Os.Tester так и с Os.Trader без измнений. Он очень прост. Мы не изменяем его с каждым релизом и поддерживаем в нём обратную совместимость.

*Одинадцать подключений на сегодня*

1) Квик 

    а) DDE. Старое и хардовое подключение, проверенное временем.
	
    б) LUA. Новое и технологичное подключение. Шлём лучи поддержки: https://github.com/finsight/QUIKSharp, которые принимали участие в создании подключения своим кодом.
	
2) СмартКом
3) Плаза 2
4) Interactiv Brokers
5) Ninja Trader
6) ASTS Bridge, он же Micex TEAP
7) Bitmex - биржа криптоВалют
8) Kraken - биржа криптоВалют
9) BitStamp - биржа криптоВалют
10) Binance - биржа криптоВалют
11) OANDA - форекс

*В комплекте с OsEngine идёт более 30ти встроенных роботов*

1) классические трендовые роботы, вроде пересечения машек, стратегии Билла Вильямса или трендовой стратегии Джесси Ливермора.

2) контрТрендовые системы на боллинжере, линиях баланса и даже некоторые маркет-мэйкерские стратегии.

3) арбитражные стратегии для торговли расхождения коррелирующих инструментов, в том числе одноногие арбитражи.

Как пользоваться и писать ботов смотрите на канале: https://www.youtube.com/channel/UCLmOUsdFs48mo37hgXmIJTQ/videos

Форум: http://o-s-a.net/forum

Вливайся!



