# Путеводитель АПС для ИВТ

![](../technical/Pic/gus_gr.svg)

Привет, студент!

Это путеводитель по дисциплине «Архитектуры процессорных систем». Здесь ты найдёшь ссылки на всю информацию генерируемую в данном курсе: конспекты лекций, методички по лабораторным работам, дополнительные материалы и литературу, популярные материалы, ссылку на облако, способы связи с преподавателями (включая анонимный) и тому подобное. Имея доступ к этой страницы ты имеешь доступ ко всему курсу АПС.


## Мотивация

30–40 лет назад, когда персональные компьютеры были ещё в новинку, а интернета как такового не было, пионеры вычислительной техники предсказывали, что в будущем электронные чипы станут настолько дешёвыми, что они будут повсюду — в домах, в транспорте, даже в человеческом теле. Для того времени эта идея казалась фантастической, даже абсурдной. Персональные компьютеры тогда были очень дороги и в большинстве своём даже не подключались к интернету. Мысль о том, что миллиарды крохотных чипов когда-нибудь будут во всем и станут дешевле семечек, казалась нелепой. Сегодня эти мысли уже не кажутся фантастическими. В последнее десятилетие почти всегда, какой-нибудь компьютер или компьютеры находятся на расстоянии вытянутой руки от человека. Билетик в метро – тоже компьютер, который спроектировал, возможно, выпускник ИВТ.

Если ты выпускник направления Информатика и Вычислительная Техника, то скорее всего, в будущем, ты будешь разрабатывать электронику, компьютеры – цифровые автоматические устройства, которые, как правило, управляются процессорами и ПЛИС. Типичное современное электронное устройство – это набор датчиков физических величин, которые посылают свои измерения в процессор, который обрабатывает полученную информацию согласно заданной программе. Понимать, как это работает также разумно, как и терапевту знать из каких органов состоит человек, несмотря на то, что он не хирург и внутрь не полезет. Выпускник ИВТ понимающий устройство компьютера будет способен разрабатывать более эффективные решения: более быстрые, точные, энергоэффективные.

Логика такая: "Чтобы разрабатывать электронику, я должен понимать из чего она делается", "Современными электронными устройствами управляют процессоры" ⟹ "Чтобы разрабатывать электронику, я должен разбираться в процессорах".


## Лекции

Весь цикл лекций можно условно разделить на 5 основных модулей. На  **основах** вводятся основные понятия дисциплины и рассматриваются используемые инструменты. Модуль **цифровой схемотехники** посвящен видам и способам построения различных функциональных блоков и узлов процессора. В модуле **архитектура и микроархитектура** процессора, на примере архитектуры RISC-V реализуется три способа построения микроархитектуры, после чего сравниваются и обсуждаются способы повышения производительности, классифицируются существующие архитектуры процессоров. Блок **процессорные системы** рассматривает основные элементы процессорных систем: память, коммуникация, ввод/вывод. На **современных архитектур процессорных систем** разбираются примеры коммерческих компьютеров различных классов применения, обсуждаются метрики эффективности и производительности. Каждый конспект сопровождается ссылками на подробные материалы, запись лекции, популярные и дополнительные материалы.

**[Основы]**

1. [Вводная](Lectures/01.%20Introduce.md)
2. [Основные концепции и инструменты](Lectures/02.%20Instruments.md)

**[Цифровая схемотехника]**

3. [Цифровая арифметика. Арифметико-логическое устройство](Lectures/03.%20Digital%20arithmetics.md)
4. [Операционные устройства](Lectures/04.%20Operations%20units.md)
5. [Последовательностная логика. Память](Lectures/05.%20Sequencial%20logic.md)

**[Архитектура и микроархитектура]**

6. [Архитектура RISC-V](Lectures/06.%20RISC-V%20architecture.md)
7. [Программирование RISC-V](Lectures/07.%20RISC-V%20programming.md)
8. [Однотактный процессор](Lectures/08.%20Singlecycle%20processor.md)
9. [Многотактный процессор. Устройство с микропрограммным управлением](Lectures/09.%20Multicycle%20processor.md)
10. [Конвейерный процессор](Lectures/10.%20Pipeline%20processor.md)
11. [Конфликты конвейера](Lectures/11.%20Pipeline%20hazards.md)
12. Методы повышения производительности
13. Виды и классификация архитектур

**[Процессорные системы]**

14. Подсистема прерываний
15. Память
16. Кэш-память
17. Виртуальная память. Операционные системы
18. Когерентность кэша. Синхронизация
19. Шины
20. Ввод/вывод

**[Современные архитектуры процессорных систем]**

21. Микроконтроллеры (на примере PIC и ARM)
22. Системы общего назначения
23. GPU и параллельные вычисления
24. Эффективность и производительность


## Лабораторные работы

Курс *Архитектур процессорных систем* включает в себя цикл из 8 лабораторных работ, в течение которых используя язык описания аппаратуры **Verilog HDL**, с нуля, последовательно, создается система на основе **FPGA** (ПЛИС, программируемая логическая интегральная схема), под управлением процессора с архитектурой **RISC-V**, управляющего периферийными устройствами и программируемого на языке высокого уровня **C**. [Подробнее](Labs/README.md) о лабораторных работах.

Список работ направления подготовки ИВТ [в квадратных скобках указаны номера лекций, в которых поднимаются соответствующие темы]:
1. [ALU](Labs/1.%20Arithmetic-logic%20unit/README.md) (Арифметико-логическое устройство) – [Лекции 3]
2. [RF](Labs/2.%20Register%20file%20and%20memory/README.md) (Регистровый файл и память) – [Лекция 5]
3. [MD](Labs/3.%20Main%20decoder/README.md) (Основной дешифратор команд) – [Лекция 8]
4. [DP](Labs/4.%20Datapath/README.md) (Тракт данных) – [Лекции 6–8]
5. [LSU](Labs/5.%20Load-store%20unit/README.md) (Блок загрузки и сохранения) – [Лекция 19]
6. [IS](Labs/6.%20Interrupt%20subsystem/README.md) (Подсистема прерывания) – [Лекция 15]
7. [PU](Labs/7.%20Peripheral%20units/README.md) (Периферийные устройства) – [Лекция 20]
8. [Programming](Labs/8.%20Programming/README.md) (Программирование на C)

Полезное дополнение к лабораторным:
- [Как установить Vivado](Other/Install%20Vivado.md)
- [Создание базового проекта с прошивкой ПЛИС в Vivado](Other/Vivado-trainer.md)
- [Что такое язык описания аппаратуры HDL](Other/What%20is%20HDL.md)
- [Конструкции языка Verilog](Other/Verilog%20syntax.md)


## Дополнительные материалы

- [Список основных определений](Other/Basic%20definitions.md)
- [Хочу под ПЛИС](Other/About%20FPGA.md)


## Облако ☁️

Основным хранилищем "габаритных" учебных и методических материалов является  [ОБЛАКО](https://1drv.ms/u/s!AlYsTGjsjfIfhP4GhdRLPQzK60vqGw?e=qKQz3L) . На данный момент в облаке находятся:

1. Презентации лекций (отдельные папки для каждого потока)
2. Методические материалы и презентации лабораторных работ (также находятся в этом репозитории)
3. Вся используемая литература 


## Обратная связь и преподаватели

[Преподаватели АПС](Other/Teachers.md) - в этой статье ты найдешь информацию о всех людях задействованных в организации проведения этой дисциплины, их контакты и расписание консультаций. 

Любые комментарии, критика, жалобы, замечания, да все что угодно, что может как-то улучшить курс, или что не нравится в текущем положении вещей, обратная связь, в любой момент времени, **анонимно** —  [сюда](https://forms.gle/Y1Dtn6EWydFxxzYXA) !


## Место АПС в Computer Science

В оригинальном видео [Map of Computer Science](https://www.youtube.com/watch?v=SzJ46YA_RaA) Доминик Уоллиман предлагает, безусловно неполную, но удобную для представления обширной области знаний, карту компьютерных наук. Ниже, на этой карте, отмечена зона, которую покрывает предлагаемый курс лекций и лабораторных работ.

Эта `COMPUTER ENGINEERING` дисциплина главным образом уделяет внимание компьютерным архитектурам, и всем взаимосвязанным вопросам в этом контексте: производительность, компиляторы, операционные системы, виртуальные машины, параллельные вычисления, ПЛИС. Такая дисциплина является важным связующим звеном между теоретическими компьютерными науками и ее приложениями, представленными в нижней части карты. Компьютерная инженерия – неотъемлемая часть в реализации современных приложений. АПС закладывает необходимую инженерную базу, наборы понятий и концепций в отношении цифровых технологий и устройств.

![](../technical/Pic/cs.png)

---


## Обзор тематической литературы

**Митио Сибуя и Такаси Тонаги**  

*Центральный процессор. Образовательная манга*

Самый лайтовый вариант усвоения основных концепций изучаемой дисциплины. Про архитектуру процессора в виде ~~комикса~~ манги. По сюжету девушка Каиураги Дюми, чемпион по японским шахматам сёги, встречает незнакомца, который предлагает ей сыграть с компьютером. Конечно же она сливает партию. И понеслось. Слово за слово и вот он уже рассказывает ей, как работает обыгравший ее компьютер. Не понять просто невозможно. А прочитав эту мангу любая книга ниже станет понятна абсолютно любому читателю. Манга  [продается](https://dmkpress.com/catalog/manga/978-5-97060-507-3/)  как в электронном, так и в печатном виде.

![](../technical/Pic/manga.jpg)

---

**Чарльз Петцольд**  

*Код. Тайный язык информатики*

Книга для тех, кому плохо пошел материал. Очень, очень классно рассказывается что такое цифровые устройства, как это работает и зачем это все нужно. На примере фонариков, азбуки Морзе, шрифта Брайля и штрих-кодов автор знакомит нас с основами кодирования информации. Из лампочек и батареек сначала собираются разные вроде бы пустяковые устройства, которые позже превращаются в полноценный компьютер. Отличная популярная литература. Если ты знаешь человека, которому с трудом дается понимание цифровой техники, то ты просто обязан порекомендовать ему эту книгу. В образовательных целях можно ознакомиться с ней в облаке. Почитать восхищенный отзыв о книге и ее содержании можно [тут](https://habr.com/ru/post/68365/). А дождаться, когда она начнет снова продаваться можно [тут](https://www.ozon.ru/context/detail/id/125884/). Либо поискать в магазинах.

![](../technical/Pic/code.jpg)

---

**Дэвид М. Харрис и Сара Л. Харрис**

*Цифровая схемотехника и архитектура компьютера: RISC-V*

Потрясающая книга, являющаяся более доступным вариантом изложения и иллюстрации книги "Архитектура компьютера и проектирование компьютерных систем", Паттерсона и Хеннесси. На примере архитектуры **RISC-V** рассказывается как построить процессор начиная с вопросов работы транзистора. Рассматриваются базовые конструкции языков описания аппаратуры **SystemVerilog** и **VHDL**. Эту книгу на чистом энтузиазме перевели на русский язык группа ученых и инженеров из стран бывшего СССР с подачи [Юрия Панчула](http://panchul.com/about_ru/). Электронный вариант для архитектуры **MIPS** распространяется бесплатно и абсолютно легально. Обязательна к ознакомлению каждому! Гораздо удобнее использовать печатный вариант, на этот случай ее можно приобрести  [тут](https://dmkpress.com/catalog/electronics/circuit_design/978-5-97060-961-3/). Электронный вариант с архитектурой **MIPS** доступен в облаке.

![](../technical/Pic/harris.png)

---

**Дэвид М. Харрис и Сара Л. Харрис**  

*Цифровая схемотехника и архитектура компьютера.  
Дополнение по архитектуре ARM*

Как и следует из названия, эта книга дополняет предыдущие описанием отличий архитектуры **ARM** от **MIPS** и **RISC-V**. Книга состоит из глав, посвященных архитектуре процессоров **ARM**, их микроархитектуре, описанию подсистемы памяти и системы ввода-вывода. Также в приложении приведена система команд **ARM**. Почему такое пристальное внимание этой архитектуре? Потому что это одна из самых массово используемых архитектур в мире. Например, 98% всех мобильных телефонов работают на процессорах с архитектурой **ARM**. Книги в облаке нет, но ее можно приобрести [тут](https://dmkpress.com/catalog/electronics/circuit_design/978-5-97060-650-6/).

![](../technical/Pic/arm.jpg)

---

**под редакцией Романова А.Ю. и Панчула Ю.В.**

*Цифровой синтез: практический курс*

В дополнение к Харрисам отлично идет практический курс цифрового дизайна, в том числе, как раз, от того самого Юрия Панчула. Книга ориентирована в первую очередь на практику создания цифровой аппаратуры на ПЛИС с помощью **Verilog HDL**. Затрагиваются вопросы процесса создания **ASIC**. Очень хорошо написана, грамотно структурирована и имеет много полезной информации, требующейся на практике дизайнеру цифровой аппаратуры. Купить можно [тут](https://dmkpress.com/catalog/electronics/circuit_design/978-5-97060-850-0/)

![](../technical/Pic/digitaldesign.png)

---

**Д. Паттерсон и Дж. Хеннесси**  

*Архитектура компьютера и проектирование компьютерных систем*

Отцы архитектуры **RISC** делятся накопленным опытом. Не только рассказывают, как процессоры работают, но и как их построить, прививают принципы проектирования, красиво указывают на заблуждения, дают хитрые задания, да и вообще книга богата полезной информацией. Нетленка. Не зря на лицевой стороне книги написано _классика computer science_. Заканчивается книга разбором многоядерных, многопроцессорных параллельных систем. Если решишь поставить к себе на полку, то придется подождать когда она  [вновь поступит в продажу](https://www.ozon.ru/context/detail/id/7425447/) или поискать на полках магазинов.

![](../technical/Pic/patterson1.jpg)

---

**Д. Паттерсон и Дж. Хеннесси**

*Архитектура компьютера. Количественный подход*

Дополнение к предыдущей книге, вся суть которой передана в названии. Рассматривается эффективность современных вычислительных машин в численном эквиваленте. Что и как влияет на производительность вычислительных систем и какие существуют зависимости. Уделяется большое внимание построению иерархии памяти и анализу результатов, исследуется параллелизм исполнения команд. В некотором смысле это библия анализа вычислительных систем. Авторы получили за нее премию Тьюринга. Рекомендуется к прочтению после прослушивания курса Архитектуры процессорных систем. В облаке лежит часть книги для ознакомления, а ее  [физическая копия](https://www.ozon.ru/context/detail/id/35204637/) хорошо дополнит домашнюю библиотеку computer science.

![](../technical/Pic/patterson2.jpg)

---

**С.А. Орлов и Б.Я. Цилькер**

*Организация ЭВМ и систем*

Фундаментальный курс по архитектуре и структуре современных компьютерных систем, написанный двумя опытными профессорами из питерских вузов. Книга написана излишне сухо, в советской манере, порой с излишним формализмом даже там, где этого можно было избежать. Однако, книга изобилует большим объемом полезной информации, богатым списком источников, в основном зарубежных. Рекомендуется использовать ее как дополнительное справочное пособие. В ней можно найти много оригинальной информации, не содержащейся в другой отечественной печатной продукции. Купить книжку можно, например, [здесь](https://www.ozon.ru/context/detail/id/147603179/).

![](../technical/Pic/orlov.jpg)

---

**Д.Н. Беклемишев, А.Н. Орлов, А.Л. Переверзев, М.Г. Попов, А.В. Горячев, А.И.Кононова**  

*Микропроцессорные средства и системы. Курс лекций*

Курс лекций, читавшийся несколько лет назад. На данный момент книга является актуальной, но дисциплина организована несколько иначе. Из достоинств можно выделить хорошую организацию написанного материала, представленного в виде одинаковых порций разбитых на тематические лекции. Книга доступна в облаке и в университетской библиотеке. Отдельно стоит отметить, что часть читаемого на лекциях материала представлена только в этом издании.

![](../technical/Pic/vt.jpg)

---

**Э. Таненбаум и Т. Остин**  

*Архитектура компьютера*

![](../technical/Pic/tanenbaum.jpg)

Книга для изучения компьютерной архитектуры от всемирно известного специалиста в области информационных технологий, писателя и преподавателя, выходящая уже в шестом издании и посвящена структурной организации компьютера. В качестве примеров архитектур рассматриваются **Intel Core i7**, **Texas Instrument OMAP4430** и **Atmel ATmega168**. Книга рассчитана на широкий круг читателей, так что можешь читать ее без опасения что что-то не поймешь, хотя не все с этим согласятся, некоторым (включая автора этих строк) книга [не нравится](https://habr.com/ru/post/589091/). Чувствуется влияние того, что Таненбаум чаще взаимодействует с цифровой аппаратурой в роли программиста, а не разработчика. Вероятно это поможет в освоении материала обучающимся на соответствующих специальностях. Купить книгу можно [тут](https://www.piter.com/collection/all/product/arhitektura-kompyutera-6-e-izd-2).

---

**Дональд Томас**

*Логическое проектирование и верификация систем на SystemVerilog*

Тем, кто не только пытается разобраться в принципах работы компьютера, но и сам хочет разрабатывать цифровые устройства потребуется более серьезно изучить какой-нибудь современный язык описания аппаратуры. Сходу, многие посоветуют SystemVerilog – наиболее популярный вариант в индустрии. Он является более современной версией Verilog, лишенной некоторых его недостатков.

![](../technical/Pic/svbook.png)

---

`Дорогу осилит идущий`
