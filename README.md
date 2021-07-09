# TGblockchain 
![TGblockchain](logo.png "TGblockchain")

https://techgensociety.com

## Build
1. install scala
2. sbt
3. rpm:packageBin
4. create temporary folder: mkdir /tmp/techgen
5. install crated in (2) rpm: sudo rpm -ivh /path/to/rpm
6. run in background: /usr/bin/bd-app &
7. see logs in /tmp/techgen 


## Краткое описание блокчейна TGblockchain 
Проект блокчейна TGblockchain состоит из двух частей:
1. Блокчейн
2. Оборзреватель блоков
Непосредственно блокчейн TGblockchain представляет собой цепочку криптографически-связанных блоков. Для разработки данного блокчейна были выбраны проверенные временем решения классических блокчейнов. Однако, широко-распространенные блокчейны имеют ряд проблем, которые при отсуствии решений приведут в будущем к деградачии базы блокчейна. На текущий момент решения появились, однако их внедрение для работающего блокчейна задача не тривиальная и требующая значительных ресурсов. Гораздо больших нежели на создание нового блокчейна с современными решениями.
Эти решения позволили получить ряд преимуществ перед традиционными широко-известными блокчейнами. Перечислим эти преимущества вкратце:

1. Нет необходимости совершать бессмысленную работу во время производства блоков или “майнинга”. 

2. Возможность гибкой настройки и контроля количества производителей в зависимости от конфигурации сети. Это позволяет уменьшить латентность сети, тем самым делая сеть более устойчивой к атакам на консенсус.

3. Возможность создания системы прав. Система прав уже позволяет проектировать простую бизнес логику на этапе создания сети. Подавляющее большинство блокчейнов не имеет системы прав и ограничивается разрешением производства блоков ноде на базе характеристик самой ноды. 

4. Возможность идентификации аккаунта. Это очень важный с юридической точки зрения момент. В последнее время одним из важных аспектов работы блокчейна стала деанонимизация пользователя. Все чаще используется механизм KYC и все чаще государственные регуляторы высказывают негативное отношение анонимным действиям в блокчейне. Также хватает кейсов и в бизнесе, когда необходимо знать пользователя. Казалось бы решение очевидное. Разрешить пользоваться блокчейном только тем пользователям, которых мы знаем. Однако такой подход слишком жесткий и некоторые потенциальные пользователи могут просто отказаться от использования такого блокчейна. Поэтому деанонимизация должна быть постепенной. Блокчейн TGblockchain предлагает другую схему. Важные действия, например такие как производство блоков будут требовать идентификации пользователя. Поскольку, возможно, за производство блоков владелец ноды будет получать прибыль. А пользователи, которым достаточно перемещать средства между аккаунтами, могут оставаться без идентификации до тех пор пока не захотят больше прав в системе. В дальнейшем такой аспект можно буде ругулировать.

5. Блокчейн TGblockchain использует технические решения, которые позволяют сократить размер кода, а следовательно и скорость внесения изменений. К примеру один из наиболее известных блокчейнов занимает более 100 000 строк кода. И это только ядро. Естественно, поддержка и разработка такого объема кода требует огромных ресурсов. Технические решения, которые используются в TGblockchain в несколько раз уменьшают кодовую базу, а следовательно и необходимый на поддержку ресурс, что крайне важно для бизнеса.

6. Возможности разработки смарт-контрактов. Функциональная парадигма является более подходящей и что самое важное более безопасной для написания смарт-контрактов. Этот вывод основан на опыте использования существующих реализаций смарт-контрактов. К сожалению, на текущий момент смарт-контракты и языки на которых они пишутся усложняются. Что приводит к тому что программисты заняты больше проблемами описания того или иного действия в технических терминах. Т.е. они думают о том как написать а не что написать. Такой подход уводит технологию из бизнеса, что существенно сказывается на количестве успешных приложений, которые реально работают для решения современных проблем. Функциональная парадигма же сосредоточена именно на описании самой логики программы, что является ее явным преимуществом.  На текущий момент блокчейны со смарт-контрактами с функциональной парадигмой только-только начали появляться. Поскольку блокчейн TGblockchain использует функциональную парадигму, то и разработка смарт-контрактов описанного типа будет логичной и бесшовной, а сами контракты станут более компактными, понятными и будут ориентированы на написание самой бизнес-логики, а не на том как описать технически эту бизнес логику. Такой подходы был выбран, чтобы изначально заложить большой потенциал развития в блокчейн TGblockchain.  

7. На сегодняшний день уже появились практические решения на базе функциональной парадигмы. Более того такие блокчейны имеют общие библитеки и уже используют функциональную парадигму в написании смарт-контрктов, что подтверждает практическую ценность выбранного подхода. В блокчейне TGblockchain используются проверенные  другими блокчейнами на практике библиотеки.

8. Оптимизации производства блоков тогда, когда это требуется. Мы видим, что иногда в блокчейнах консенсуса PoA появляются путые блоки. Это происходит из-за слишком частой генерации блоков, которая независит от заполняемости транзакциями. Таким образом мы заполняем базу путыми записями. А все мы знаем какие размеры баз имею современные блокчейны. TGblockchain может генерировать блоки в зависимости от заполняемости блокчейна. Что позволит избежать пустых блоков и настроить оптимальное соотношение скорости выполнения транзакций к заполняемости блоков. 

9. В блокчейне TGblockchain заложена техническая возможность работать с несколькими активами.

Рассмотрим решения, которыми достигаются указанные преимущества более детально:

### Консенсус
Блокчейн TGblockchain работает на базе консенсуса Proof Of Authority. Такой подход дает ряд преимуществ по сравнению с более распространенными консенсусами. Сравним.
Proof Of Work довольно изученный и стабильный консенсус. Однако, использует вычислительные мощности в пустую и порой требует значительного времени на производство блоков. Proof Of Stake - владение долей. Он хоть и не заставляет майнера выполнять бесполезную работу, но недостаточно изучен, имеет ряд технических проблем и сложен в реализации и тестировании. 
Наиболее подходящим является Proof Of Authority. Не выполняет лишней работы, проще в реализации чем Proof Of Stake, не так уязвим и предоставляет гибкость в назначении производителя, если блокчейн приватный, скорость существенно выше. Основной недостаток такого консенсуса - слабая децентрализация. Однако, на примере широко-распространенных блокчейнов мы знаем, что реальная децентрализация не такая как заявляют пользователям. Как правило есть некоторое количество крупных майнеров, контролирующих сеть. В блокчейне TGblockchain децентрализацию можно контролировать количеством нод.  И она не сильно будет отличаться от реальной ситуации с широко-известными блокчейнами.

### Настройка производителей
Кол-во производителей можно настраивать с помощью транзакций ноды с соответствующими правами. Это позволяет быстро менять конфигурацию в целях достижения минимальной латентности сети при максимальном количестве нод. 
	Нода, обладающая правом добавления или удаления производителя из консенсуса отправляет транзакцию. Как только транзакция попадёт в цепочку блоков, так другие производители начнут обновлять свой список нод.  И уже на основе этого списка будут фильтровать новые блоки. 

### Система прав
Система прав предполагает что БЧ начинает работать при создании суперноды. Нода которая имеет полный список прав. Далее владелец ноды реализует механизм делегации прав. Предполагается что минимальный набор прав, необходимый для функционирования 
ноды следующий:

1. Право на производство блоков
2. Право на делегацию производства блоков
3. Право на делегацию права делегации производства блоков
	
  Конечно это всего-лишь базовый список на основе которого нода сможет начать работать. У классических блокчейнов, к сожалению, система прав отсутствует. Потому переход уже существующих БЧ на систему прав крайне ресурсоемкий. Только недавно в единицах блокчейнов начали появляться системы прав. Такая система является существенными преимущество и качественным скачком вперед по сравнению с другим блокчейнами. 
В блокчейне TGblockchain разработка системы прав довольна проста, потому как технология рассчитана на расширения. 
Система прав позволяет в некоторых случаях  реализовать простую бизнес логику для клиентов на этапе доработки БЧ . Приведем пример реализации системы прав. Например, можно реализовать право на управление средствами вашего аккаунта. Таким образом без необходимости доступа к паролю вашего аккаунта может быть введено внешнее управление. Такой кейс в классических блокчейнах требует написания смарт-контрактов в лучшем случае или даже написания байткода. Естественно когда клиент обычный пользователь, а не программист, он не имеет возможности воспользоваться такой логикой. Система прав же позволяет существенно снизить порог входа не некоторых бизнес-кейсах и увеличить привлекательность БЧ.

### Идентификация
Как мы уже писали ранее в современном мире идентификация является важным юридическим аспектом, а также может служить причиной в отказе от совершения каких-либо действий в соответствии с заложенной в блокчейне бизнес-логикой. 
Запрет на использование БЧ пользователями не прошедшими идентификацию не является выходом. Потому как такое решение чревато массовым отказом пользователей от использования БЧ и высоким порогом входа (один из известных блокчейнов с аналогичным консесусом имеет такую проблему и она сильно влияет на массовое распространение). 
В TGblockchain необходимо избавить пользователя от проблем при знакомстве с блокчейном. Т.е. с одной стороны нужно оставить возможность простой регистрации и в то же время предоставить возможность идентификации по желанию, если пользователю требуются специфичные действия. Как например - производство блоков. 
Эту проблема в TGblockchain решается следующим образом. Если пользователь хочет пересылать средства, ему достаточно сгенерировать публичный и приватный ключ. Это действие в одно нажатие кнопки на веб-сервисе. Тем самым порог входа мы оставили максимально простым.
Если же пользователь хочет стать производителем блоков, то ему необходимо пройти идентификацию. Один из механизмов - покупка в системе идентификатора. Плата за идентификатор позволит избежать массовой генерации идентификаторов при отсутствии иных ограничений.
Таким образом мы получаем гибкий механизм, который с одной стороны избавляет БЧ от усложнений при входе пользователя, а с другой стороны позволяет идентифицировать пользователя при необходимости. 
К сожалению, на текущий момент блокчейнов с такой же гибкой системой нет.

### Технология
Как мы уже писали ранее в написании TGblockchain использованы современные технологии, которые позволили в разы уменьшить кодовую базу, повысить безопасность и упростить разработку. 
Кодовая база большинства блокчейнов является форком уже существующих. А существующие были написаны на языках, создававшихся преимущественно в прошлом веке.  
На сегодняшний день у нас есть возможность писать на языках, которые специально создавались для решения подобных задач. Наш выбор пал на язык Scala. Опишем преимущества:

1. Проектировался именно для того чтобы решать задачи масштабируемости было просто и поэтому из коробки имеет соответствующие инструменты.
2. Новые языки имеют существенный недостаток! Отсутствие большого кол-ва библиотек, которые были написаны для старых языков на протяжении многих лет. Но в Scala такой проблемы нет. Дело в том что Scala обратно совместима с виртуальной машиной Java. А все мы знаем что язык Java это простой промышленный язык, который держиться в первых строчках по популярности уже много лет и в основном используется в бизнесе и банковской сфере. Таким образом библиотеки Java и Scala совместимы. Мы можем использовать библиотеку Scala из Java и наоборот.
3. Язык Scala совмещает несколько парадигм: объектно-ориентированную и функциональную. В наше время разработчики все чаще смотрят в сторону функциональной парадигмы. И не просто так. Ведь этот подход позволяет избежать массы ошибок при многопоточном программировании. 
4. Существенное уменьшение кодовой базы. Если сравнивать Scala с C или c Java, то решение одной и той же задачи на Scala требует написания кода в 2 или даже в 5 раз меньше. 
5. Scala имеет статическую типизацию. Это значит что многие ошибки можно выявить на этапе компиляции. 
6. Опыт решения рутинных задач работы с структурами данных в Java был учтен при проектировании Scala. Поэтому многие задачи, которые в Java решались написанием рутинного кода, в Scala решаются одной строчкой. Готовые решения повседневных задач означают что программисту не приходится постоянно писать почти один и тот же код в котором даже из-за банальной невнимательности можно допустить ошибки.
7. Решена проблема множественного наследования. В Scala можно гибко комбинировать функционал для классов, в то время как в Java в некоторых случаях приходилось этот функционал дублировать, что приводило к увеличению кодовой базы и потенциальной возможности допустить ошибку при исправлении такого функционала.

Это далеко не все преимущества выбранной технологии. Однако все эти преимущества сводятся к трем самым важным для бизнеса: уменьшение времени на создание продукта, уменьшение стоимости и увеличение производительности. Также эксперты сходятся во мнении, что функциональная парадигма является очевидно подходящим решением для решения задач блокчейна.

### Производительность
В понятие производительности входят прежде всего два фактора. Кратко обозначим их относительно реализации в блокчейне TGblockchain:
1. Количество произведенных блоков за единицу времени - иначе говоря скорость производства блоков. Поскольку мы имеем дело с консенсусом, которые не зависит от работы производителя, то теоретически скорость ограничена только мощностью машины производителя. А поскольку технически даже относительно слабый и не современный компьютер способен производить больше блоков чем того требует современный уровень развития, то скорость можно считать неограниченной технологией самого блокчейна. Что является существенным преимуществом выбранного консенсуса. 
2. Объем транзакции в блоке - объем транзакций в блоке технически не ограничен в реализации блокчейна TGblockchain.

Но, следует понимать, что оба этих фактора хоть и практически не ограничены в реализации самого блокчейна, но имеют ограничения в других местах. А именно. Первый и в особенности второй фактор существенно зависят от пропускной способности сетевого соединения, его качества и от латентности. И если мы поставим в блоке бесконечное кол-во транзакций, то можем забить сеть, а как следствие допустить атаку на консенсус. Такая же ситуация обстоит и с блоками. Если мы будем генерировать огромное кол-во блоков в сети, то другие участники сети не будут успевать синхронизироваться и тем самым сеть будет расходится. Поэтому в целях безопасности в блокчейне существует возможность гибкой настройки этих параметров. Как правило эти параметры выбираются относительно текущего развития интернета в момент тестирования сети. В момента запуска эти параметры уже назначаются постоянным и в дальнейшем могут меняться только в форка. 
Однако, очевидно что постоянное производство блоков может приводить к появлению пустых блоков. В этом случае блокчейн TGblockchain имеет возможность строить оптимизацию. Если кто-то решил заработать на пустом блоке, то сеть его отклонит. Такая реализация позволит оптимизировать занимаемое блоками место в блокчейне TGblockchain. Однако стоит иметь в виду что конечные параметры выбираются в зависимости от целей и тестирования сети. К примеру,  в некоторых сетях идет счет времени по кол-ву блоков.
Итак, блокчейн TGblockchain не ограничен в консенсусе скоростью производства блоков, в отличие от блокчейнов типа Proof Of Work. Все остальные параметры настраиваются в результате тестирования и подстройки сети.

### Эффективность
Как мы писалил ранее под эффективностью мы понимаем соотношение скорости выполнения транзакций и заполяемости блоков. Мы можем генерировать блоки и тысячу разв  секунду и больше. Это уже зависит от производительности вычислительного комплекса, на котором стоит узел. Однако, если блокчейн у нас обсулживает большое кол-во транзакций. Блоки генериуются по 10 раз в секунду. А их заполняемость не более 50%. И при этом блоки достаточно маленькие для передачи по сети. То в этом случае логично встроить механимз динамического или статического (на базе прав блокчейна) регулирования заполняемости блоков и скорости их генерации. Такой механизм позволяет быстро адаптировать блокчейн к меняющимся потребностям бизнеса. К примеру, для платежных транзакций важна больше скорость, а для подписи и хранения информации. 

### Архитектураня поддержка реализации новых активов
Создание и тестирование смарт-контрактов является очень трудоемкой задачей. Однако, мы знаем, как важно иметь возможность поддерживать токены бизнес-проектов. Современные  блокчены стермятся поддержать монеты без смарт-контрактов на ранних этапах развития. Что позволяет делать свопы (перемщения откенов с одного блокчейна на другой) монеты. А это очень важно для популяризации молодого болкчейна. В TGblockchain архитектурно заложена возможность реализации такого механизма. 
 
 

