# Rational Unified Process

**Rational Unified Process (RUP)** є ітеративним процесом розробки програмного забезпечення створеним Rational Software — підрозділом IBM з 2003. RUP не є єдиним, конкретним розпорядчим процесом, а скоріше фреймворком процесу, що має бути адаптованим організаціями які займаються розробкою та командами розробників які оберуть елементи процесу, які підходять під їх потреби.

## Історія

**Rational Unified Process (RUP)** являє собою продукт, спочатку розроблений Rational Software, яка була придбана компанією `IBM` в лютому 2003 року. Продукт містить у собі базу знань з гіперпосиланнями, та прикладами артефактів і докладні описи для різних видів діяльності. RUP входить в продукт IBM Rational Method Composer (RMC), який дозволяє налаштування процесу.

До 1997 року, Rational придбав Verdix, Objectory, Requisite, SQA, Performance Awareness, та Pure-Atria. Поєднання баз досвіду цих компаній привело до вироблення семи «найкращих практик» сучасної програмної інженерії:

- Розробляти ітеративно, керуючись ризиками.
- Управляти вимогами
- Використовувати компонентну архітектуру
- Моделювати програмне забезпечення візуально
- Постійно перевіряти якість
- Контролювати зміни
- Підлаштовуватись


Ці найкращі практики рухали розробку продуктів Rational, та використовувались польовими командами Rational, щоб допомогти клієнтам вдосконалити якість, та передбачуваність їх розробницьких зусиль. Щоб зробити ці знання доступнішими, Філіпу Крачтену, було поставлено завдання збирати явні фреймворки сучасної розробки програмного забезпечення. Ці зусилля використовував заснований на HTML механізм доставки процесів розроблений Objectory. У результаті «Раціональний уніфікований процес» (RUP) завершив стратегічну опору для Rational:

- Адаптовний процес що направляє розробку
- Інструменти, що автоматизують використання цього процесу
- Сервіси, що прискорюють впровадження і процесу, і інструментів.



## Теми Раціонального Уніфікованого Процесу

### Будівельні блоки RUP

RUP заснований на наборі будівельних блоків, чи містить елементи, що описують те, що повинно бути зробленим, необхідні навички, та покрокове пояснення того, як досягаються конкретні цілі розробки. Основними будівельними блоками, чи елементами вмісту, є наступні:

- Ролі (хто). Роль визначає набір навичок, компетенції та відповідальності.
- Робочі продукти (що). Робочий продукт являє собою щось отримане з завдання, в тому числі всі документи і моделі, випущені під час роботи впродовж процесу.
- Завдання (як). Завдання описує одиницю роботи, яка доручена ролі, яка забезпечує значущий результат.
- У кожній ітерації, завдання діляться на дев'ять дисциплін: шість «інженерних дисциплін» (бізнес-моделювання, вимоги, аналіз і проектування, реалізація, тестування, розгортання) і трьох допоміжних дисциплін (конфігурація і керування змінами, управління проектами, середовища).


### Чотири фази життєвого циклу проекту

![RUP](images/RUP_process.png)

RUP визначає життєвий цикл проекту, що складається з чотирьох фаз. Ці фази дозволяють процесу, бути представленим на високому рівні, подібно до того як представляються проекти у «водоспадному» стилі, хоча, по суті, ключем до процесу є ітерації розробки, які простягаються вздовж всіх фаз. Крім того, кожен етап має одну ключову ціль, та віху в кінці, яка позначає досягнення цілі.


- ##### Початкова фаза
	Первинною ціллю є адекватна оцінка системи, як база для обчислення початкових розцінок та бюджету. На цьому етапі встановлюються бізнес випадки, які включають бізнес-контекст, фактори успіху (очікувані доходи, визнання на ринку, і т.д.), а також фінансовий прогноз. На додаток до бізнес випадку генерується базова модель прецедентів, план проекту, попередня оцінка ризику і опис проекту (основні вимоги до проекту, обмеження та основні характеристики). Після їх завершення проект перевіряється на відповідність наступним критеріям:

	- Зацікавлені сторони досягають згоди з визначення масштабів і оцінки вартості/термінів.
	- Розуміння вимог як свідчення якості первинних прецедентів.
	- Достовірність оцінок вартості/термінів, пріоритетів, ризиків, та процесу розробки.
	- Глибина і ширина будь-якого архітектурного прототипу, який був розроблений.
	- Встановлення базової лінії за допомогою якої можна порівняти фактичні витрати із запланованими витратами.

	Якщо проект не пройде цей етап, що називається віхою життєвого циклу, він може бути як скасований так і повторений після переконструювання з метою кращого задоволення критеріїв.


- ##### Фаза уточнення

	Основна мета полягає в пом'якшенні ключових ризиків, виявлених на основі аналізу до кінця цієї фази. Фаза уточнення — фаза де проект починає набувати форми. На цьому етапі робиться аналіз предметної області, і архітектура проекту отримує свою базову форму.

	Ця фаза має пройти віху життєвого циклу архітектури (LCA), задовольняючи такі критерії:

	- Модель прецедентів, в якій ідентифікуються прецеденти та актори, та розробляється більшість описів прецедентів. Модель прецедентів повинна бути завершена на 80%.
	- Опис архітектури програмного забезпечення в процесі розробки програмної системи.
	- Виконувана архітектура, яка реалізує архітектурно значимі прецеденти.
	- Бізнес — випадки та список ризиків переглядаються.
	- План розвитку проекту в цілому.
	- Прототипи, що явно зменшили кожен виявлений технічний ризик.
	Якщо проект не може переступити цю віху, ще є час для того, щоб він був скасований або змінений. Тим не менше, після закінчення цього етапу, проект переходить в операцію з високим ступенем ризику, де зміни набагато складніші та згубні, при здійсненні.

	Системна архітектура є ключовим елементом розробки, що отримується з аналізу предметної області.


- ##### Фаза конструювання

	Основна мета полягає в створенні програмної системи. На цьому етапі основна увага приділяється розробці компонентів та інших характеристик системи. Це етап, коли відбувається основна частина кодування. У більш великих проектах, може бути кілька фаз конструювання, в спробі поділити прецеденти на керовані сегменти, які можуть утворити презентабельні прототипи.

	Цей етап створює перший реліз програмного забезпечення. Його завершення позначає віха початкової боєготовності.

- ##### Фаза впровадження

	Основна мета полягає в переведенні системи з розробки у продукт, зробивши її доступною та зрозумілою для кінцевого споживача. Діяльність у рамках цієї фази включає навчання кінцевих користувачів та обслуговуючого персоналу, бета-тестування системи для перевірки її на відповідність очікуванням користувачів. Продукт також перевіряється на відповідність рівню якості, встановленого в початковій фазі.

	Якщо всі вимоги задоволені, досягається віха релізу продукту, і цикл розробки завершується.