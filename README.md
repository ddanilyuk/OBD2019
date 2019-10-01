# OBD2019


## Структура бази даних системи управління проектами (БД СУП).

## Методологіі проектування програмного забезпечення

Метою проектування є визначення внутрішніх властивостей системи і деталізації її зовнішніх (видимих) властивостей на основі виданих замовником вимог до ПО (вихідні умови задачі). Ці вимоги піддаються аналізу.
Проектування ПЗ включає такі основні види діяльності:

- вибір методу і стратегії вирішення;
- вибір представлення внутрішніх даних;
- розробка основного алгоритму;
- документування ПЗ;
- тестування і підбір тестів;
- вибір представлення вхідних даних.

Спочатку програма розглядається як чорний ящик. Хід процесу проектування і його результати залежать не тільки від складу вимог, а й обраної моделі процесу, досвіду проектувальника.

Залежно від класу створюваного ПЗ, процес проектування може забезпечуватися як «ручним» проектуванням, так і різними засобами його автоматизації. В процесі проектування ПЗ для вираження його характеристик використовуються різні нотації - блок-схеми, ER-діаграми, UML-діаграми, DFD-діаграми, а також макети.

Проектуванню зазвичай підлягають:

- Архітектура ПЗ;
- Пристрій компонентів ПЗ;
- Призначені для користувача інтерфейси.

Проектування ведеться поетапно відповідно до стадій:

Технічне завдання;
Технічна пропозиція;
Ескізний проект;
Технічний проект;
Робочий проект.

На кожному з етапів формується свій комплект документів, званий проектом (проектною документацією).


База даних, в загальному випадку, здійснює інтеграцію даних, створюючи динамічно (в реальному масштабі часу) оновлювану модель предметної області (проекту) у вигляді єдиного для всіх завдань блоку даних. Спрощено кажучи, структура БД - це  таблиці і їх зв'язки, що містяться в БД. Структура БД дозволяє підтримувати логіку кожного конкретного завдання, що виконується над збереженими даними і підтримує можливість організації даних з точки зору уявлення користувача.
Структура БД СУП є ключовим робочим продуктом, необхідним при роботі з проектом. Вона являє собою ієрархічний перелік робочих дій, необхідних для створення проекту і роботи з ним. Структура утворює свого роду каркас, на основі якого проектується всі компоненти проекту.
Таким чином, БД СУП призначена для створення ієрархічних зв'язків між елементами проекту і робочими діями (елементами процесу) і містить наступні елементи (типова структура):
1. Вихідні дані, базові процеси і граничні умови проекту: ресурси (об'єкти, які необхідні в процесній діяльності (персонал, обладнання та ін.); Призначення (зв'язок певного завдання і ресурсів, необхідних для її виконання. Вона дозволяє розрахувати обсяг часу, що витрачений на проект, його вартість для проекту, виробляти динамічний перерозподіл ресурсів); час, вартість, обсяг робіт; завдання (робота, здійснювана в рамках проекту для досягнення певного результату, яка повинна бути завершена протягом деякого періоду часу); фази (збори пов'язаних завдань, в процесі виконання яких реалізується виробництво певного продукту. Якщо для досягнення результатів завдання потрібно виконати тільки його, то для досягнення результату фази потрібно виконати групу інших завдань. Фази також служать для зручності контролю робіт);
2. Встановлення зв'язків між даними, обмежень, фільтрів, що дозволяють структурувати і спільно використовувати дані для опису процесів - формування (планування) проектів різного масштабу (проектів, мультипроекта, підпроектів). Створення плану проекту полягає в описі його ключових характеристик (тривалість, робочий час, методика планування); задач проекту і зв'язків між ними (в MS Project підтримується 4 типи зв'язків: закінчення-початок, початок-початок, закінчення-закінчення, початок-закінчення); доступних ресурсів і визначення взаємозв'язку між ними за допомогою призначень: обмежень (прив'язування завдань до певних дат); крайніх термінів (гранична дата виконання завдання); вартості; сумарного завдання проекту, що об'єднує всі проектні активності).
До типових наборів властивостей завдання проекту відносяться: тривалість завдання; трудовитрати; призначені ресурси; обмеження; крайні терміни; пріоритет (важливість її виконання для проекту).
До типових наборів властивостей ресурсів проекту відносяться: вартість; завантаження; доступність; призначення; пріоритет.
Для роботи з БД СУП в MS Project використовуються інтерфейс і шаблони.


## 2. Користувацький інтерфейс (види уявлень інформації про проект, панелі інструментів).

### 2.1. Види представлення інформації про проект.

Представлення - це спосіб відображення проектних даних для перегляду та редагування. Micrisoft Progect містить наступні види представлень інформації про проекти (складових представлення): таблиці (листи), діаграми і форми. Файл проекту містить величезну кількість даних, і переглядати їх одночасно неможливо. У представленні на екрані відображається обмежений набір потрібної інформації про проект, що полегшує її перегляд і редагування. Представлення має гнучку структуру і може складатися як з окремої таблиці, діаграми або форми, так і з їх комбінації.
Представлення може бути одне або як комбінація декількох (діаграма Ганта, лист ресурсів і т. Д.) І, у разі необхідності, таблиці або фільтра. Представлення дозволяють працювати з інформацією в різних форматах.
Менеджмент процесу (що розуміється як послідовність кроків, тобто ряду дій і операцій, спрямованого на досягнення певної мети) починається з проектного (організаційного) підходу. Зовнішній інтерфейс процесу охоплює всю інформацію, яка може використовуватися для його визначення. Для організації, що склалася при цьому забезпечується представлення основ знань попереднього проекту, методів вимірювання продукту і інших параметрів. Для нової організації або організації, яка є "новою" в рамках процесу, інтерфейс являє області, які треба "відвідати" з метою збору інформації та даних, необхідних для запуску проекту.
Таблиці - це одне з основних засобів представлення проектних даних в MS PROJECT.
Типи таблиць MS Project
У проектному файлі всі дані зберігаються у вигляді двох таблиць, одна з яких тримає інформацію про завдання, а друга - про ресурси проекту, тобто про задіяних у виконанні завдань людях і матеріальних цінностях. Ці дві "внутрішні" таблиці складають основу файлу проекту і складаються з безлічі полів, більшість з яких створено "про запас" і зазвичай не використовуються. Деякі з них можуть бути задіяні при програмуванні, в тонких налаштуваннях, функціях аналізу проекту і т.д., але не потрібні при стандартному використанні MS PROJECT. Під час роботи над проектом, як правило, потрібні певні зрізи інформації. Наприклад, дані про вартість проекту, завантаженості чи інших ресурсів, терміни закінчення робіт по поточним завданням і т.п. Тобто в кожен конкретний момент часу потрібно мати перед очима необхідну інформацію. Це дозволяє сконцентруватися на ній і ефективно працювати.
Файл проекту складається з двох великих "внутрішніх" таблиць з безліччю стовпців, з яких тільки деякі відображаються в таблицях, включених в представлення. Робота в MS Project, відбувається в основному тільки з маленькими "зовнішніми" таблицями. В MS Project закладено набір визначених таблиць, призначений для роботи з невеликим обсягом проектної інформації (табл. 1 і 2 Додатка) з цих таблиць і містить лише кілька полів однієї з "внутрішніх" таблиць проектного файлу. Відповідно, "зовнішні" таблиці (як і "внутрішні) містять інформацію або про завдання, або про ресурси.
Таким чином, "всередині" MS Project є таблиця ресурсів і таблиця завдань, а "зовні", в інтерфейсі, є ряд таблиць, які є набором полів або з однієї, або з іншої "внутрішньої" таблиці.
Діаграми.
Діаграма є графічним засобом відображення, що міститься в проектному файлі інформації. З діаграми можна отримати візуальне уявлення про послідовність завдань, їх відносної тривалості, про тривалість проекту в цілому. В MS PROJECT діаграми є не тільки засобом перегляду проектної інформації, але з їх допомогою можна вводити нові дані і редагувати існуючі.
Діаграма Ганта представляє собою засіб для подання тривалості і послідовності завдань в проекті. Так, всі елементи діаграми Ганта - основного засобу візуалізації плану проекту (час - завдання) в програмі є налаштованими відрізками, кожен з яких може складатися з 3 елементів: точки початку, точки закінчення і проміжної частини (при цьому будь-який з елементів може бути відсутнім). При стандартному налаштуванні відрізки, що позначають фази, складаються з усіх трьох елементів. Відрізки, що позначають завдання, складаються тільки з проміжної частини, а завершальні задачі - тільки з початкової точки.
На діаграмі Ганта поруч з відрізками може відображатися додаткова інформація (наприклад, на малюнку поруч із завданнями, відображаються назви задіяних в них ресурсів і їх завантаження при виконанні завдання). Склад цієї інформації визначається налаштуваннями діаграми, в MS PROJECT входить кілька заздалегідь налаштованих версій діаграми Ганта, на яких поруч з відрізками відображається різна інформація (Табл. 3 Додатка).
MS PROJECT, крім діаграми Ганта, містить 3 мережевих графіка (або блок-схеми): власне Network Digram (мережевий графік), Discriptiv Network Digram (мережевий графік з описом), і Relationship Digram (схема даних або діаграма залежностей). Відмінність мережевого графіка з описом від стандартного мережевого графіка полягає тільки в підвищеній інформативності блоків У них обох можна відразу переглядати інформацію про весь план проекту, а на схемі даних - тільки про одну завдачу цього плану; вона призначається для аналізу взаємозв'язків між задачами.
Одна з основних діаграм при роботі з MS PROJECT - Calendar (Календар), за допомогою якого подається план робіт у вигляді традиційного календаря. Діаграма Календар відображає інформацію про план проекту у вигляді таблиці з сімома або п'ятьма колонками, відповідними дням тижня, і безліччю рядів, відповідним тижням. Задачі на календарі позначаються відрізками, які починаються в день початку робіт над задачею і закінчуються в день її закінчення.
Діаграма Resourse Graph (Графік ресурсів) містить інформацію про різні аспекти участі ресурсів у проекті: виконуваній роботі, процентному завантаженні, можливості виконувати інші завдання крім тих, на які вони вже виділені, і вартості. За допомогою цієї діаграми можна порівнювати участь в проекті декількох ресурсів або ресурсу і групи ресурсів, що робить її потужним аналітичним інструментом. Група ресурсів відбирається шляхом фільтрації, за замовчуванням в якості групи виступають всі ресурси проекту. Змінивши умови фільтрації, можна змінити і склад групи. Дані можна переглядати як для групи в цілому, так і для будь-якого окремого ресурсу всередині групи.
Діаграми використання задач і ресурсів більшою мірою, ніж інші, застосовуються для введення почасових даних в файл проекту.
Діаграма Task Usage (Використання задач) призначена для аналізу участі ресурсів у проектних роботах. Сама діаграма являє собою таблицю, в рядках якої розміщена інформація про фази, задачі і ресурси. Усередині рядка дані розміщені в осередках відповідно з датами, до яких вони належать. Таким чином діаграма дозволяє отримати різноманітні дані про роботу (обсяг роботи, вартість, завантаження ресурсів та ін.) за довільний часовий період для проекту в цілому, будь-який з його фаз, задач або задіяного у виконанні задач ресурсу. Діаграма Resource Usage (Використання ресурсів) призначена для аналізу за будь-який період часу як загального завантаження ресурсу в проектних роботах, так і з яких завдань вона складається.
Форми.
Форма - це засіб відображення і редагування проектних даних в Project, який може бути включений до складу представлення. За допомогою форм можна переглядати інформацію тільки про один об'єкт (ресурс або задачу), але при цьому можна редагувати майже всі його властивості.
В MS PROJECT входять п'ять форм. За допомогою перших двох можна переглядати і редагувати інформацію про ресурси, а трьох наступних - про задачі: Resoure Form (Форма ресурсів); Resoure Name Form (Форма назв ресурсів); Task Form (Форма задач); Task Name Form (Форма назв задач); Task Details Form (Форма відомостей про задачі).

### 2.2. Створення нових представлень.

Щоб створити нове представлення, в діалоговому вікні зі списком представлень потрібно клацнути по кнопці New (Створити). У вікні, визначається тип створюваного представлення: Single view (Одиночне представлення) або Combination view (Комбіноване представлення). Після вибору типу нового представлення відкривається діалогове вікно визначення його властивостей. Залежно від того, яке представлення створюється, буде відкрито діалогове вікно визначення властивостей одиночного або комбінованого представлення.
У діалоговому вікні визначення властивостей одиночного представлення, в поле Name (Ім'я) вказується назва нового представлення. Ця назва потім з'явиться в списку всіх представлень і в меню, якщо встановити прапорець Show in menu (Показувати в меню). Список, що розкривається Screen (Екран) дозволяє вибрати діаграму або форму, яка ляже в основу представлення. Перелік доступних варіантів обмежується розглянутими діаграмами і формами. Від пункту, обраного в списку Screen (Екран), залежить, які параметри буде налаштовано для створюваного представлення. Список Table (Таблиця) доступний тільки в разі, якщо обраний екран містить таблицю. У цьому списку можна вибрати таблицю, яка буде відображатися при завантаженні представлення. Список Group (Група) також доступний тільки в тому випадку, якщо діаграма допускає угруповання даних. Тоді можна вибрати в списку групу, яка буде використовуватися при угрупованні. Умови фільтрації даних можна визначити для будь-якої діаграми за допомогою списку Filter (Фільтр), в якому перераховані існуючі фільтри, призначені для відбору даних, що відображаються у представленні . Для того щоб використовувати фільтрацію в режимі виділення, призначений прапорець Highlight filter (Виділяти результати фільтра). Якщо цей прапорець встановлений, будь-які фільтри, які в подальшому будуть застосовуватися до даного представлення, також працюватимуть тільки в режимі виділення.
Діалогове вікно визначення властивостей комбінованого представлення, влаштовано простіше аналогічного вікна для одиночного представлення. В поле Name (Ім'я) слід ввести назву нового представлення, а для того, щоб показати його в меню і на панелі представлення, потрібно встановити прапорець Show in menu (Показувати в меню). У списках, що розкриваються Тор (вгорі) і Bottom (внизу) вибираються представлення, які будуть відображатися у верхній і нижній частинах нового представлення. При цьому список доступних представлень полягає не тільки з стандартних діаграм (як в діалоговому вікні створення одиночного представлення), а з набору існуючих одиночних представлень, в тому числі і налаштованих користувачем.
Після того, як створення представлення завершено, воно з'являється в списку доступних представлень і його можна викликати або зі списку, або (якщо встановлений відповідний прапорець) з меню або панелі уявлень.

### 2.3. Створення нового представлення на основі існуючого.

Часто зручніше створювати нове представлення не «з нуля", а на базі вже існуючого. Для цього клацанням по кнопці Copy (Копіювати) в діалоговому вікні зі списком представленm виконується копіювання виділеного в списку представлення. Після клацання по кнопці Copy (Копіювати) відкривається діалогове вікно, схоже на вікно створення представлення. У цьому вікні до назви вихідного представлення додається Copy of (Копія), а на місці списку Screen (Екран) розташовується інформаційне поле, що не дає можливості змінити діаграму або форму, яка є базовою для скопійованого представлення. Після клацання по кнопці ОК представлення з новою назвою зберігається.

