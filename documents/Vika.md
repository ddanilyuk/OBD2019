
## Методології проектування програмного забезпечення

Метою проектування є визначення внутрішніх властивостей системи і деталізації її зовнішніх (видимих) властивостей на основі виданих замовником вимог до ПЗ (вихідні умови задачі). Ці вимоги піддаються аналізу. Проектування ПЗ включає такі основні види діяльності:

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

- Технічне завдання; 
- Технічна пропозиція; 
- Ескізний проект; 
- Технічний проект; 
- Робочий проект.

На кожному з етапів формується свій комплект документів, званий проектом (проектною документацією).

Проектування ПЗ - це процес визначення архітектури, набору компонентів, їх інтерфейсів, інших характеристик системи і кінцевого складу програмного продукту.

Область знань «Проектування ПЗ (Software Design)» складається з таких розділів:

- базові концепції проектування ПЗ (Software Design Basic Concepts),
- ключові питання проектування ПЗ (Key Issue in Software Design),
- структура й архітектура ПЗ (Software Structure and Architecture),
- аналіз і оцінка якості проектування ПЗ (Software Design Quality Analysis and Evaluation),
- нотації проектування ПЗ (Software Design Notations),
- стратегія і методи проектування ПЗ (Software Design Strategies and Methods).

Базова концепція проектування ПЗ - це методологія проектування архітектури за допомогою різних методів (об'єктного, компонентного й ін.), процеси ЖЦ (стандарт ISO/IEC 12207) і техніки - декомпозиція, абстракція, інкапсуляція й ін. На початкових стадіях проектування предметна область декомпозується на окремі об'єкти (при об'єктно-орієнтованому проектуванні) або на компоненти (при компонентному проектуванні). Для подання архітектури програмного забезпечення вибираються відповідні артефакти (нотації, діаграми, блок-схеми і методи).

Ключові питання проектування - це декомпозиція програм на функціональні компоненти для незалежного і одночасного їхнього виконання, розподіл компонентів у середовищі функціонування і їх взаємодія між собою, забезпечення якості і живучості системи й ін.

Проектування архітектури ПЗпроводиться архітектурним стилем, заснованим на визначенні основних елементів структури - підсистем, компонентів, об'єктів і зв'язків між ними.

Архітектура проекту - високорівневе подання структури системи і специфікація її компонентів. Архітектура визначає логіку системи через окремі компоненти системи настільки детально, наскільки це необхідно для написання коду, а також визначає зв'язки між компонентами. Існують і інші види подання структур, засновані на проектуванні зразків, шаблонів, сімейств програм і каркасів програм.

Один з інструментів проектування архітектури - патери (шаблон). Це типовий конструктивний елемент ПЗ, що задає взаємодію об'єктів (компонентів) проектованої системи, а також ролі і відповідальності виконавців. Основна мова опису - UML. Патерн може бути структурним, що містить у собі структуру типової композиції з об'єктів і класів, об'єктів, зв'язків і ін.; поведінковим, що визначає схеми взаємодії класів об'єктів і їх поведінку, задається діаграмами адитивностей, взаємодії, потоків керування й ін.; погоджувальним, що відображає типові схеми розподілу ролей екземплярів об'єктів і способи динамічної генерації структур об'єктів і класів.

Шаблон проектування або патерн (англ. Design pattern) в розробці програмного забезпечення - повторювана архітектурна конструкція, що представляє собою рішення проблеми проектування в рамках деякого контексту.

Зазвичай шаблон не є закінченим зразком, який може бути прямо перетворений в код; це лише приклад розв'язання задач, який можна використовувати в різних ситуаціях. Об'єктно-орієнтовані шаблони показують відносини і взаємодії між класами або об'єктами, без визначення того, які кінцеві класи або об'єкти додатка будуть використовуватися.

«Низькорівневі» шаблони, що враховують специфіку конкретної мови програмування, називаються ідіомами. Це хороші рішення проектування, характерні для конкретної мови або програмної платформи, і тому не універсальні. На найвищому рівні існують архітектурні шаблони, вони охоплюють собою архітектуру всієї програмної системи.

Основна користь від використання шаблонів полягає в зниженні складності розробки за рахунок готових абстракцій для вирішення цілого класу проблем. Шаблон дає рішенням своє ім'я, що полегшує комунікацію між розробниками, дозволяючи посилатися на відомі шаблони. Таким чином, за рахунок шаблонів проводиться уніфікація деталей рішень: модулів, елементів проекту, - знижується кількість помилок. Застосування шаблонів концептуально так як і використання готових бібліотек коду. Правильно сформульований шаблон проектування дозволяє, відшукавши вдале рішення, користуватися ним знову і знову. Набір шаблонів допомагає розробнику вибрати можливий та найбільш підходящий варіант проектування.

Аналіз і оцінка якості проектування ПЗ - це заходи щодо аналізу сформульованих у вимогах атрибутів якості, функцій, структури ПЗ, з перевірки якості результатів проектування за допомогою метрик (функціональних, структурних і ін.) і методів моделювання і прототипування.

Нотації проектування дозволяють представити опис об'єкта (елемента) ПЗ і його структуру, а також поведінку системи. Існує два типи нотацій: структурна, поведінкова, та множина їх різних представлень.

Структурні нотації - це структурне, блок-схемне або текстове подання аспектів проектування структури ПЗ з об'єктів, компонентів, їх інтерфейсів і взаємозв'язків. До нотацій відносять формальні мови специфікацій і проектування: ADL (Architecture Description Language), UML (Unified Modeling Language), ERD (Entity-Relation Diagrams), IDL (Interface Description Language) тощо. Нотації містять y собі мовний опис архітектури й інтерфейсу, діаграм класів і об'єктів, діаграм сутність-зв'язок, конфігурації компонентів, схем розгортання, а також структурні діаграми, що задають у наочному вигляді оператори циклу, розгалуження, вибору і послідовності.

Поведінкові нотації відбивають динамічний аспект роботи системи та її ком­понентів. Ними можуть бути діаграми потоків даних (Data Flow), діяльності (Activity), кооперації (Colloboration), послідовності (Séquence), таблиці прийняття рішень (Décision Tables), передумови і посту мови (Pre-Post Conditions), формальні мови специфікації (Z, VDM, RAISE) і проектування.

Стратегія і методи проектування ПЗ. До стратегій відносять: проектування вгору, вниз, абстрагування, використання каркасів і ін. Методи є функціонально-орієнтовані, структурні, які базуються на структурному аналізі, структурних картах, діаграмах потоків даних й ін. Вони орієнтовані на ідентифікацію функцій і їх уточнення знизу-вгору, після цього уточнюються діаграми потоків даних і проводиться опис процесів.

В об'єктно-орієнтованому проектуванні ключову роль відіграє спадкування, поліморфізм й інкапсуляція, а також абстрактні структури даних і відображення об'єктів. Підходи, орієнтовані на структури даних, базуються на методі Джексона [12] і використовуються для подання вхідних і вихідних даних структурними діаграмами. Метод UML призначений для опису сценаріїв роботи проекту у наочному діаграмному вигляді. Компонентне проектування ґрунтується на використанні готових компонентів (reuse) з визначеними інтерфейсами і їх інтеграції в конфігурацію, як основи розгортання компонентної системи для її функціонування в операційному середовищі.

Формальні методи опису програм ґрунтуються на специфікаціях, аксіомах, описах деяких попередніх умов, твердженнях і постумовах, що визначають заключну умову одержання правильного результату програмою. Специфікація функцій і даних, якими ці функції оперують, а також умови і твердження — основа доведення правильності програми.

