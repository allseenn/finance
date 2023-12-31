# ФИНАНСОВАЯ МАТЕМАТИКА
**Финансовая математика** – это основа всей современной теории экономики и финансов.

## 1. ВРЕМЕННАЯ СТОИМОСТЬ ДЕНЕГ TVM (Time Value of Money)

### КОНЦЕПЦИЯ ВРЕМЕННОЙ СТОИМОСТИ ДЕНЕГ

Сумма денежных средств, доступная в настоящий момент, имеют большую ценность (стоимость), чем эта же сумма в какой-то момент времени в будущем. Чем раньше мы получаем деньги, тем это выгоднее для нас!

### ПРОСТЫЕ И СЛОЖНЫЕ ПРОЦЕНТЫ

**Процентная ставка** (interest rate) – это количественное отражение временной стоимости денег, которая может интерпретироваться как:
- **Ставка доходности** (rate of return), которую требует инвестор, чтобы вложить деньги в данную инвестицию
- **Альтернативная стоимость** (т.н. «вмененные издержки») – альтернативные возможности вложений для конкретного инвестора
- **Ставка дисконтирования** – это параметр, который используется для сравнения денежных сумм в разные моменты времени.

Процентная ставка бывает двух видов:
1. **Простая процентная ставка** (simple interest rate) – применяется только к основной сумме долга
2. **Сложная процентная ставка** (compound interest rate) - учитывает начисление процентов на всю сумму, включая ранее начисленные проценты (с капитализацией).


### ДИСКОНТИРОВАНИЕ И НАРАЩЕНИЕ

**i** (interest rate) - процентная ставка за один период

**n** (number of years) - период выплат (каждый год)

**m** (number of compounding periods per year) - периодичность, т.е. количество выплат в течении периода (внутри года)

**PV** (Present Value of money) - Текущая стоимость денег (В excel ПС() - приведенная стоимость)

**FV** (Future Value of money) - Будущая стоимость денег (В excel БС() - будущая стоимость)

**Дисконтирование** – процесс перевода денежной суммы от будущего момента времени к прошлому
<table border=1>
<tr><th>Простая процентная ставка</th><th>Сложная процентная ставка</th></tr>
<tr><td> 

$$PV=\frac{FV}{1+in}$$
</td><td>

$$PV=\frac{FV}{(1+i)^n}$$
</td></tr>
</table>

**Наращение** - процесс перевода денежной суммы от прошлого момента к будущему
<table border=1>
<tr><th>Простая процентная ставка</th><th>Сложная процентная ставка</th></tr>
<tr><td> 

$$FV=PV(1+in)$$
</td><td>

$$FV= PV(1+i)^n$$
</td></tr>
</table>

**Выгоды максимально частой капитализации процентов** - в зависимости от условий начисления процентов при одной и той же процентной ставке эффект (то есть, итоговая сумма) будет различным!
<table border=1>
<tr><th>Наращение для начисления процентов по сложной ставке i в течении n периодов</th>
<th>Дисконтирование для начисления процентов по сложной ставке i в течении n периодов</th></tr>
<tr><td> 

$$FV=PV(1 + \frac{i}{m})^{nm}$$
</td><td>

$$PV=FV(1+\frac{i}{m})^{nm}$$
</td></tr>
</table>

**Эффективная процентная ставка** - та процентная ставка, которая дает тот же эффект с точки зрения итоговой денежной суммы, но при условии начисления 1 раз в год
$$FV = PV(1+эф.ставка)$$

### СТАВКА ДИСКОНТИРОВАНИЯ
**Ставка дисконтирования** представляет собой отражение концепции временной стоимости денег, которая проистекает из трех основных источников:
- **Инфляция**
- **Премия за риск** 
- **Безрискова ставка**

#### Инфляция
**Инфляция** – падение покупательской способности денег во времени
Инфляция может быть определена как 
1. падение покупательской способности денег во времени; либо как 
2. стабильный рост цен на определенный набор товаров и услуг (“потребительскую корзину”) в экономике

**Потребительская корзина** - набор товаров и услуг, характеризующий уровень и структуру потребления экономического субъекта

Когда в экономике присутствует инфляция, то стоимость денег в стране возрастает и процентные ставки становятся выше.

##### Уравнение Фишера
**Реальная процентная ставка** (Rреал)- процентная ставка, очищенная от инфляции

**Номинальная процентная ставка** (Rном) - та процентная ставка, которая зафиксирована в договоре (например, кредита или депозита)
$$(1 + Rном) = (1 + Rреал) (1 + I)$$

#### Премия за риск
**Риск** - измеримая возможность наступления неблагоприятных финансовых последствий (потери всех или части инвестированных денег) в результате неопределенности:
- кредитные риски
- риски ликвидности
- рыночный риск

**Неопределенность** - отсутствие точной информации о будущем развитии событий, течении процессов и финансовых результатах

И если в сделке есть риск, то для осуществления этой сделки требуемая доходность будет включать в себя эту премию за риск.

#### Безрисковая ставка

Чтобы субъект был готов отложить потребление и инвестировать свои деньги (то есть временно расстаться с ними), ему нужно взамен предложить какую-то дополнительную, ненулевую доходность, которую и называют безрисковой ставкой.

В любой экономической ситуации любой рациональный субъект при любых условиях будет предпочитать получить деньги раньше, а не позже, то есть для него деньги имеют временную стоимость!

### ПРИМЕРЫ ЗАДАЧ К РАЗДЕЛУ 1
[Задачи в экселе](01.Lecture/lec01.xlsx)

## 2. РАСЧЕТОВ ПРОЦЕНТОВ

### ДЕНЕЖНЫЕ ПОТОКИ И АННУИТЕТЫ

**Денежный поток** – реальное движение денежных средств проекта в виде набора денежных сумм с привязкой к конкретным моментам времени. У каждой составляющей денежного потока есть три параметра: денежная сумма, момент времени и знак.

Если мы получаем деньги, то для нас эта сумма идет со знаком "+", если мы платим, то со знаком "-"

Для инвестиционных проектов: в начале идет т.н. **инвестиционная фаза**, когда нам приходится вкладывать деньги, а затем начинается **операционная фаза**, когда мы начинаем зарабатывать деньги.

Денежные потоки нерегулярны во времени. Но, часто, мы имеем дело с т.н. аннуитетом

**Аннуитет** (annuity) - денежный поток, элементы которого равны между собой и поступают или уплачиваются через равные промежутки времени
Аннуитеты можно встретить в самых разных областях экономики и финансов:
· графики погашения кредитов и лизинга;
· договора финансовой ренты;
· платежи по облигациям;
· платежи от сдачи в аренду квартиры и т.д.

**Финансовая рента** - соглашение, в соответствии с которым одна сторона (получатель ренты) передает другой стороне (плательщику ренты) в собственность имущество, а плательщик ренты обязуется в обмен на полученное имущество периодически выплачивать получателю ренты определённую денежную сумму

Виды аннуитетов:
1. **Аннуитет постнумерандо** (ordinary annuity) - когда платеж по аннуитету происходит в конце периода.
2. **Аннуитет пренумерандо** (annuity due) - когда платеж по аннуитету происходит в начале каждого периода.
3. **Перпетуитет** - бесконечный аннуитет

#### Формулы для расчета аннуитетов 
Они основаны на геометрической прогрессии.
**PV** - текущая (приведенная) стоимость аннуитета
**FV** - будущая стоимость
**n** - период
**A** - платеж
**r** - ставка дисконтирования (стоимость денег)

#### Аннуитет постнумерандо 

$PV=A\frac{1-(1+r)^{-n}}{r}$

$FV=A\frac{(1+r)^n-1}{r}$

#### Аннуитет пренумерандо 

$PV=A\frac{1-(1+r)^{-n}}{r}(1+r)$

$FV=A\frac{(1+r)^n-1}{r}(1+r)$

#### Перпетуитет (perpetuity)

$PV = \frac{A}{r}$

### ОБЛИГАЦИИ

**Облигация** - ценная бумага, которая представляет собой долговое обязательство, т.е. обязательство периодически платить в течение срока проценты по заданной ставке (купоны) и в конце срока уплатить основную сумму долга (номинал облигации).

Бывают облигации, которые не платят процентов (купонов), а только возвращают долг в конце срока – такие облигации называют бескупонными.

Облигация имеет два параметра
1. Справедливую цену
2. Доходность

Цена облигации определяется как приведенная стоимость будущих денежных потоков по облигации

Доходность облигации определяется как ставка дисконтирования, которая приравнивает приведенную стоимость будущих денежных потоков по облигации к ее фактической рыночной цене.

### КРЕДИТЫ

**Кредит** – банковская операция по предоставлению денежных средств заемщику на условиях возвратности (возврата всей суммы в оговоренный срок), платности (уплаты процентов на взятую в долг сумму), и срочности (установления четкого срока кредита)

**График погашения** - расписание всех платежей по кредиту с выделением сумм процентов и сумм погашения основного долга на весь срок кредита

Есть два способа составления графика погашения:
· с фиксацией ежемесячных платежей (чаще всего, аннуитетных)
· с фиксацией графика погашения основной суммы долга

### ЛИЗИНГ
Существуют два вида лизинга: 
- операционный
- финансовый

**Операционный лизинг** - по сути, обычная долгосрочная аренда.

**Финансовый лизинг** – договор, согласно которому лизинговая компания предоставляет имущество в пользование заемщику на длительный срок (сравнимый со сроком жизни этого имущества) и предоставляет заемщику право (либо обязательство) выкупить имущество в конце срока договора.

Сумма, за которую в конце можно выкупить оборудование, называется **выкупной суммой** (выкупной стоимостью).

### ПРИМЕРЫ ЗАДАЧ К РАЗДЕЛУ 2
[Задачи в экселе](02.Lecture/lec02.xlsx)


## 3. ОЦЕНКА ЭФФЕКТИВНОСТИ ИНВЕСТИЦИЙ

### ИНВЕСТИЦИОННЫЕ ПРОЕКТЫ И ОЦЕНКА ИХ ЭФФЕКТИВНОСТИ

**Инвестиционный проект** - временное предприятие, направленное на создание уникального продукта, услуги или результата (экономического или социального), посредством осуществления инвестиций (вложений денежных сумм)

Инвестиционные проекты классифицированы:
· производственные («построить завод для производства 2 000 автомобилей в месяц»);
· научно-исследовательские («изучить возможности создания назальной вакцины от коронавируса»);
· финансовые («создать систему обработки онлайн-платежей для бронирования гостиниц»);
· коммерческие («создать сеть дистрибьютеров для производителя сельскохозяйственной техники»);
· социальные («создать 1000 парковочных мест на перехватывающей парковке») и т.д.

У инвестпроектов всегда есть:
1. цель
2. срок
3. бюджет
4. измеримый результат
5. формализованные критерии оценки достижения результата

Одной из неотъемлемых частей любого анализа является определение **инвестиционной привлекательности** проекта, то есть ответ на вопрос, есть ли смысл вкладывать в этот проект, эффективен ли инвестпроект.

**Эффективность проекта** - степень соответствия результатов (фактических или прогнозных) проекта целям и интересам его участников

**Эффективность инвестиционного проекта** - соотношение финансовых результатов проекта и затрат ресурсов на его реализацию

Можно говорить об эффективности проекта для отдельных его участников, например:
· для главного организатора проекта (общая эффективность проекта)
· отдельных инвесторов (инвестиционная эффективность)
· общества (социально-экономическая эффективность)
· государства (бюджетная эффективность) и т.д.

т.е. для выгодоприобретателей (stake holders)

### ЧИСТАЯ ПРИВЕДЕННАЯ СТОИМОСТЬ NPV (ЧПС)

**Чистая приведенная стоимость** (Net Present Value, NPV) - сумма всех дисконтированных денежных потоков по проекту, приведенных к текущему моменту времени:

$$ NPV=CF_0+\frac{CF_1}{(1+k)^1}+\frac{CF_2}{(1+k)^2}+...+\frac{CF_n}{(1+k)^n}=\sum_{t=0}^{n}\frac{CF_t}{(1+k)^t}$$

где $CF_i$ - денежный поток по проекту в момент времени i и k - ставка дисконтирования.

NPV показывает, каков будет итоговый денежный результат от реализации проекта в терминах текущей стоимости денежных средств, т.е. иными словами, на сколько вырастет благосостояние инвестора при реализации проекта!

Все инвестиционные проекты, у которых NPV > 0, следует принимать, а все инвестиционные проекты с NPV < 0 – отвергать. С NPV = 0, такой проект также имеет смысл принять.

### ВНУТРЕННЯЯ НОРМА ДОХОДНОСТИ IRR (ВСД)

**Внутренняя норма доходности** или **внутренняя ставка доходности** (Internal Rate of Return, IRR) - ставка дисконтирования, при которой чистая приведенная стоимость проекта равна 0

$$NPV=0=CF_0+\frac{CF_1}{(1+IRR)^1}+\frac{CF_2}{(1+IRR)^2}+...+\frac{CF_n}{(1+IRR)^n}=\sum_{t=0}^{n}\frac{CF_t}{(1+IRR)^t}$$

IRR дает результат в виде процентной доходности, что делает процесс сравнения легче и удобней. Если сказать инвестору «проект принесет 12% годовых» - то все сразу становится понятно. Если же сказать «проект принесет 10 млн рублей», то сразу возникнут уточняющие вопросы.

Но, если сравниваем проекты, то нужно сравнивать NPV, т.к. этот показатель более уникален в деталях.

У IRR есть два существенных методологических недостатка:
- если проект имеет знакопеременные денежные потоки, то могут быть проблемы с расчетом и интерпретацией IRR
- IRR предполагает, что стоимость денег во все периоды проекта одинаковая, но в реальной жизни это не так.

### ПРОЧИЕ МЕРЫ ОЦЕНКИ ЭФФЕКТИВНОСТИ

**Ликвидность** - способность актива превращаться в деньги.

**Срок окупаемости** (Payback Period, PP) - число лет, которые уйдут на то, чтобы окупить первоначальные инвестиции в проект положительными денежными потоками от проекта:
- Является мерой ликвидности проекта
- Не учитывает терминальную стоимость проекта ( потоки за горизонтами окупаемости)

Срок окупаемости бывает:
- обыкновенным
- дисконтированным

**Индекс доходности** (Profitability Index, PI) - отношение суммы всех дисконтированных будущих положительных притоков по проекту к первоначальным инвестициям. Не зависит от размера проекта.

$$PI=1+\frac{NPV}{инвестиции}%$$

Показывает сколько рублей мы получим за каждый вложенный рубль.

Если PI > 1 (эквивалентно NPV > 0), то проект принимаем. PI < 1 - проект отклоняем

**Модифицированная внутренняя норма доходности** (Modified Internal Rate of Return, MIRR) – ставка дисконтирования, при которой чистая приведенная стоимость проекта равна 0, при условии, что все положительные денежные потоки реинвестируются по ставке реинвестирования, а все оттоки привлекаются на условиях кредита под ставку финансирования

МIRR аналог IRR, который отдельно учитывает ставку реинвестирования доходов (под какой процент нам удастся инвестировать притоки в течение проекта) и ставку финансирования инвестиций (под какой процент нам удастся взять кредит в течение проекта):

$$MIRR = \sqrt[n]{\frac{FV(положительные\:CF, ставка\:реинвестирования)}{-PV(отрицательные\:CF,\:ставка финансирования)}}-1 $$

Этот показатель был разработан, чтобы элиминировать два основных недостатка стандартного показателя IRR (риск отсутствия или множественности значений и предположение о реинвестировании потоков по проекту под ту же ставку).

### ПРИМЕРЫ ЗАДАЧ К РАЗДЕЛУ 3
[Задачи в экселе](03.Lecture/lec03.xlsx)

## 4. ПРИМЕНЕНИЕ СТАТИСТИКИ В ЭКОНОМИКЕ

### ТЕОРИЯ ВЕРОЯТНОСТЕЙ 

**Теория вероятностей** – раздел математики, изучающий случайные события, случайные величины и их свойства.
**Случайное событие** – событие, у которого нет заранее известного исхода и набор вероятных исходов у такого события всегда больше одного. Примером случайного события может быть бросок игрального кубика.
**Случайная величина** – величина, чье значение меняется в зависимости от случая (т.е. неопределенности). . Примером случайной величины может быть число очков, которое выброшено на игральном кубике.
Cлучайные величины могут быть дискретными, то есть принимать одно из определенного набора значений, или непрерывными, принимая любое значение внутри некоторого интервала.
**Вероятность** – мера возможности наступления некоторого события, которая определяется как число в интервале от 0 до 1 (где 0 означает абсолютную невозможность и 1 означает достоверность).

Вероятность события Х обычно обозначается как Р(Х). Знание вероятности позволяет найти ожидаемое значение:
$$ E(X) = X1*P(X1) + X2*P(X2) +… $$
- **Е(Х)** – ожидаемое значение величины Х;
- **Х1, Х2,** … - значения величины Х в различных исходах;
- **Р(Х1), Р(Х2),** … - соответствующие вероятности этих исходов.

Вероятность события А (например, выпадение решки при броске монеты) равна 
$$Р(A) = \frac{M}{N}$$
- **М** – число исходов (только 1 из 2 возможных результатов – это решка), когда событие А произошло
- **N** – полное число возможных исходов (2 возможных исхода – решка и орел)

Вероятность противоположного события (например, выпадения не решки при броске монеты):
$$P(не A) = 1 – P(A)$$

**Независимые события** – события, реализация одного из них никак не влияет на вероятность реализации второго (например, выпадение решки при первом броске монеты и выпадение решки при втором броске монеты):

$$P(A \;and \;B) = P(A \cap B) = P(A)P(B)$$

Внимание применяем только для независимых событий.
Если события А и Б зависимые, то используем формулу:

$$P(A \cap B) = P(A|B)*P(B)$$

**P(A and B)** – вероятность того, что произойдут одновременно события А и В.

**Несовместные события** – события, которые не могут произойти одновременно (например, выпадение орла и решки на подброшенной монете):
$$P(A\;or\;B) = P(A \cup B) = P(A)+P(B)$$
где Р(А or В) – вероятность того, что произойдет либо событие А, либо событие В.

**Общая формула сложения вероятностей**:
$$P(A\;or\;B) = P(A)+P(B) - P(A\;and\;B)$$

<img src=pics\union.png>

**Условная вероятность** – вероятность некоторого события А (например, рост акции) при условии наступления некоторого события B (например, общего роста экономики):
$$P(A|B) = \frac{P(A \cap B)}{P(B)}$$

**Теорема Байеса** представляет собой формулу для расчета условной вероятности, и описывает вероятность события А, на основе информации о некоторых условиях В, которые связаны с наступлением события:

$$P(A|B) = \frac{P(A)P(B|A)}{P(B)}$$

- P(A) - априорная вероятность гипотезы А;
- P(A|B) - вероятность гипотезы А при наступлении события В (апостериорная вероятность);
- P(B|A) - вероятность наступления события В при истинности гипотезы А;
- P(B) - полная вероятность наступления события B.

### МАТЕМАТИЧЕСКАЯ СТАТИСТИКА
 
**Математическая статистика** - раздел математики, изучающий методы описания и анализа данных наблюдений и экспериментов с целью прогнозирования случайных событий.

Все статистические методы разделяются на две категории: 
- описательная статистика (descriptive statistics) позволяет количественно описать некоторое событие или процесс
- статистика выводов (inferential statistics) позволяет на основе этого описания делать прогнозы относительно будущего развития событий.

**Генеральная совокупность** - это набор всех возможных значений, которые случайная величина принимала за все время наблюдения.

**Выборка** - некоторое подмножество исторических значений случайной величины (то есть часть генеральной совокупности).

**Функция вероятности** p(x) - зависимость вероятности появления определенного значения “x” случайной величины X от этого значения.

$$p(x)=P(X=x)$$

Функция вероятности всегда ограничена 0 и 1: 	

$$0 \leq p(x) \leq 1$$

Поскольку случайная величина гарантированно примет одно из набора ее значений, то сумма вероятностей для всех значений всегда равна 1:

$$\sum p(x) = 1$$

**Среднее значение случайной величины** (или математическое ожидание) - среднее арифметическое всех значений, которые входят в рассматриваемый период.

Матожидание для ген.совокупности:

$$\mu = \frac{\sum\limits_{i=1}^{n}*X_i}{N}$$ 

Матожидание для выборки:
$$\overline{X} = \frac{\sum\limits_{i=1}^{n}*X_i}{n} $$
**Медиана** - средняя величина в упорядоченном ряду исторических значений. 

**Мода** - то значение случайной величины, которое чаще всего встречается в историческом наборе данных.

**Геометрическое среднее** - рассчитывается по формуле:
$$G=\sqrt[n]{X_1 \times X_2 \times ... \times X_n} = (X_1 \times X_2 \times ... \times X_n)^\frac{1}{n}$$

**Гармоническое среднее** - рассчитывается по формуле:

$$ H = \frac{N}{\sum\limits_{i=1}^{N}\frac{1}{X_i}}$$

**Дисперсия** - мера разброса значений случайной величины относительно её математического ожидания.

Дисперсия ген.совокупности:

$$\sigma^2 = \frac{\sum\limits_{i=1}^{N}(X_i-\mu)^2}{N} $$

Дисперсия выборки:

$$s^2 = \frac{\sum\limits_{i=1}^{n}(X_i-\overline{X})^2}{n-1} $$

**Среднеквадратичное отклонение** (СКО) - это квадратный корень из дисперсии.

#### Законы распределения вероятности

Для непрерывных случайных величин функция вероятности р(х) не имеет смысла, поскольку возможных значений - бесконечное множество, и вероятность одного конкретного значения всегда равна 0!

Вместо этого используется функция **плотности вероятности** f(x), которая позволяет определить вероятность попадания случайной величины в определенный интервал. 

<img src=pics\DistrNorm.png>

Альтернативный способ описания распределения случайной величины, с помощью (кумулятивной) функции распределения F(x), которая показывает вероятность того, что случайная величина Х меньше или равна конкретного значения х:
$$F(x)=P(X \leq x)$$

<img src=pics\DistrCom.png>

Для описания распределения используют следующие параметры:
- Матожидание (среднее значение);
- Среднеквадратичное отклонение или дисперсия;
- Симметричность распределения относительно среднего значения.
- Эксцесс - островершинность распределения, обычно измеряется как избыточный эксцесс относительно нормального распределения 

**Симметричность распределения**:
<table>
<tr><th>скошенно влево</th><th>симметрично</th><th>скошено вправо</th></tr>
<tr><td><img src=pics\DistrLeft.png></td><td><img src=pics\DistrSem.png></td><td><img src=pics\DistrRight.png></td></tr>
</table>

**Эксцесс**:

<img src=pics\DistrAccess.png>

#### Нормальное распределение

**Нормальное распределение** (распределение Гаусса) - это наиболее часто используемое распределение случайной величины в финансово-экономических расчетах, которое имеет классический колоколообразный вид.

Основные свойства нормального распределения:
- оно полностью описывается матожиданием и среднеквадратичным отклонением;
- линейная комбинация нескольких нормально распределенных случайных величин также распределена нормально;
- “хвосты” распределения асимптотически стремятся к нулю на бесконечности

Для удобства практической работы (в том числе, с использованием таблиц распределения или формул в Excel) и сравнения используется стандартизация нормального распределения:
$$z=\frac{значение - матожидание}{СКЛ} = \frac{x-\mu}{\sigma} \sim N(0,1) $$

#### Центральная предельная теорема (закон больших чисел)

Для произвольной выборки из n значений случайной величины с матожиданием μ и дисперсией σ2, распределение среднего значения по этой выборке стремится к нормальному распределению с матожиданием μ и дисперсией σ2 / n по мере того, как растет размер выборки n.
Вне зависимости от реального распределения случайной величины для больших размеров выборки с ней можно работать как с нормальным распределением (на практике для количество данных > 30)!

### РИСК И ДОХОДНОСТЬ

**Доходность актива** - процент от стоимости актива, который инвестор заработал в результате инвестиции.
$$R(i) = \ln(\frac{P(i)}{P(i-1)}) $$
это не арифметическая доходность, а т.н. геометрическая!

Если нам нужно определить доходность за длительный период (месяц, год), то мы должны пересчитать из среднедневной доходности:
$$R_{год} = R_{дн} * 252 \;(число\;торговых\;дней)$$
Формула применяется только для малых периодов (минута, час, день). 

**Акция** - ценная бумага, подтверждающая владение частью компании (бизнеса) и право на получение дивидендов и доли имущества в компании при ликвидации.

**Дивиденды** - регулярно выплачиваемую часть прибыли компании.

Нормальное распределение не может быть использовано для моделирования цен акций, потому что цены ограничены снизу 0. Поэтому нормальным распределением моделируются доходности активов, а их цены моделируются т.н. логнормальным распределением:

<img src=pics/DistrLog.png>

**Риск** - это количественная оценка потенциальных потерь и их вероятности в силу наличия неопределенности относительно будущих событий, обычно измеряемая волатильностью (то есть, среднеквадратическим отклонением доходности актива).

В современных финансах есть целая наука - риск-менеджмент, посвященная задачам классификации, анализа, оценки и управления рисками. Однако для подавляющего большинства приложений риск называется волатильностью 

**Волатильность** - среднеквадратическим отклонением доходности актива.

### ПОРТФЕЛЬНЫЙ АНАЛИЗ

**Инвестиционный портфель** - набор финансовых активов, который управляется как единое целое, с учетом зависимостей доходности и риска отдельных активов между собой.

Вся современная теория управления портфелем была заложена двумя учеными-экономистами - Гарри Марковицем и Уильямом Шарпом. Марковиц первым математически описал эффект диверсификации.

**Диверсификация** - снижение риска инвестиционного портфеля в результате добавления в него новых активов.

Диверсификация основана на несовершенной корреляции между доходностями активов. 

Формулы Марковица для определения доходности и риска портфеля:

$$E(R_p) = r_p = w_1 r_1 + w_2 r_2 + \ldots + w_n x_n$$
$$\sigma_p^2 = w_1^2 \sigma_1^2 + w_2^2 \sigma_2^2 + 2w_1w_2\rho_{12}\sigma_1\sigma_2$$


- E(R_p) или $r_p$ доходность портфеля (portfolio) 
- $r_1$ и $r_2$ доходность конкретного актива
- $\sigma^2_p$ обозначает дисперсию (или риск) портфеля,
- $w_1$ и $w_2$ доли инвестирования в различные активы,
- $\sigma_1$ и $\sigma_2$ стандартные отклонения (риски) отдельных активов,
- $\rho_{12}$ коэффициент корреляции между рассматриваемыми активами.

<img src=pics/Markovic.png>

*горизонтальная ось – риск, вертикальная – доходность*

Без эффекта диверсификации зависимость будет иметь вид прямой линии. По мере того, как степень зависимости между доходностями акций падает (коэффициент корреляции уменьшается), прямая превращается в кривую. И мы видим следующий эффект: что мы можем получить совокупный риск портфеля из двух активов ниже, чем риск каждого из активов в отдельности!!! Именно поэтому в инвестициях есть золотое правило диверсификации: нужно составлять свой портфель из акций разных отраслей, разных стран, разных валют

Уильям Шарп первым обратил внимание на то, что потенциал диверсификации ограничен: риск не будет падать ниже определенного уровня, который он назвал рыночным или систематическим риском.

<img src=pics/Sharp.png>

Модель Шарпа позволяет найти равновесную (справедливую) доходность любого актива как функцию от чувствительности к рыночному риску (коэффициента бета):

$$E(R_i)=R_f+\beta_i[E(R{mkt})-R_f]$$

- $R_f$ безрисковая ставка
- $E(R_mkt)$ ожидаемая доходность рынка. В РФ это ММВБ-РТС.
- $\beta$ коэффициент бета данного актива

**Дериватив** — договор (контракт), по которому стороны получают право или обязуются выполнить некоторые действия в отношении базового актива. Фактически дериватив – это ценная бумага на ценную бумагу. Существует несколько основных видов производных ценных бумаг: фьючерсы, форвардные контракты, свопы, опционы, свопционы, контракты на разницу.

### ПРИМЕРЫ ЗАДАЧ К РАЗДЕЛУ 4
[Задачи в экселе](04.Lecture/lec04.xlsx)

## 5. ВВЕДЕНИЕ В ЭКОНОМЕТРИКУ

**Эконометрика** – наука, изучающая количественные и качественные экономические взаимосвязи с помощью статистических и других математических методов и моделей.

Эконометрику можно разбить на несколько областей:
- корреляционный анализ -> предназначен для качественного поиска зависимостей между экономическими случайными величинами (например, между доходностью инвестиционного фонда и доходностью рыночного индекса);
- регрессионный анализ -> предназначен для количественного определения аналитической зависимости между двумя экономическими величинами (например, поиск уравнения зависимости между ценой золота и ценой акции золотодобывающей компании);
- анализ временных рядов -> используется для прогнозирования будущих значений экономической величины на основе ее исторических значений (например, прогнозирование будущей волатильности индекса на основе его исторической динамики);
- панельный анализ -> предназначен для одновременного изучения статистических данных и во времени, и между экономическими величинами (например, анализ данных по бедности или преступности). Этот вид анализа мы не будем рассматривать.

### КОРРЕЛЯЦИОННЫЙ АНАЛИЗ

**Корреляционный анализ** — метод обработки статистических данных, с помощью которого измеряется теснота связи между случайными величинами. Корреляционный анализ является инструментом для поиска и оценки статистической зависимости.

**Статистическая зависимость** – означает, что распределение вероятностей одной случайной величины зависит от значения другой случайной величины.

Стат.зависимость может быть:
- линейной - подавляющее большинство экономических величин имеют линейную связь
- нелинейной

**Линейная корреляция (зависимость)** - мера линейной связи между двумя случайными величинами. Измеряется коэффициентом линейной корреляции Пирсона:

$$ -1 \leq r \leq +1 $$ 

<table>
<tr><th>r = +1 совершенная положительная корреляция</th><th>0 < r < +1 несовершенная положительная корреляция</th><th>r = -1 совершенная отрицательная корреляция</th><th>-1 < r < 0 это несовершенная отрицательная корреляция</th><th>r = 0 линейная зависимость отсутствует</th></tr>
<tr><td><img src=pics/CorPerfPos.png></td><td><img src=pics/CorUnPerfPos.png></td><td><img src=pics/CorPerfNeg.png></td><td><img src=pics/CorUnPerfNeg.png></td><td><img src=pics/CorNone.png></td></tr>
</table>

Чем больше значение коэффициента корреляции по модулю (чем он сильнее отличается от 0), тем сильнее линейная взаимосвязь между исследуемыми величинами.

**Ограничения корреляционного анализа:**
- требуется достаточное количество данных;
- он измеряет только линейную взаимосвязь, а статистическая взаимосвязь может быть нелинейной;
- он не позволяет выделять причинно-следственные связи;
- большое влияние оказывают “выбросы”;
- существует т.н. ложная корреляция (то есть, ситуация, когда математически корреляция есть, а экономически взаимосвязи нет).

По результатам корреляционного анализа мы можем получить информацию о наличии взаимосвязи. Однако этого мало. Нам же нужно понимать, как выглядит эта зависимость, нужна формула, чтобы мы могли ее использовать для расчетов. Именно этим инструментом и является регрессионный анализ.

### РЕГРЕССИОННЫЙ АНАЛИЗ

**Регрессия** - поиск уравнения зависимости одной случайной величины (называемой зависимой) от другой (называемой независимой), коэффициенты которого подбираются по некоторому критерию, позволяющему наилучшим образом объяснить изменение зависимой величины.

Если предполагаемое уравнение зависимости величин имеет линейный вид, то такая регрессия будет называться линейной. 

$$Y_i = \beta_0 + \beta_1X_i + \varepsilon_i, \;i=1,...n$$

- Х - независимая величина (переменная), например, цена золота; 
- Y - зависимая величина, например, цена акции золотодобывающей компании, 
- $\varepsilon$ – случайная ошибка.

Целью расчета регрессии является определение коэффициентов $\beta_0$ и $\beta_1$. Однако, точного значения этих коэффициентов мы никогда не узнаем, поскольку всегда имеем дело не с генеральными совокупностями, а с ограниченными выборками. Поэтому вместо точных значений коэффициентов мы рассчитываем их оценки:

$$\hat{Y}_i=\hat{\beta}_0+\hat{\beta}_1X_i,\; i=1,...,n$$
​
- $\hat{Y}_i$ предсказанное значение i-той зависимой переменной,
- $\beta_0$ это коэффициент сдвига (интерсепт),
- $\beta_i$ это коэффициенты регрессии для соответствующих независимых переменных 

Поиск коэффициентов линейной регрессии может осуществляться по-разному, однако в подавляющем большинстве случаев используется метод наименьших квадратов: подбираются такие коэффициенты, чтобы сумма квадратов отклонений реального значения величины Y от ее прогнозного значения согласно уравнению регрессии для всех значений величины X была минимальной. 

<img src=pics/Regression.png>

**Множественная регрессия** - поиск коэффициентов линейной зависимости одной, зависимой случайной величины от нескольких независимых случайных величин.

$$Y_i = \beta_0 + \beta_1X_{1i} + \beta_2X_{2i} +...+\beta_kX_{ki} + \varepsilon_i$$

После расчета регрессии необходимо оценить ее качество. Главным показателем качества регрессии является коэффициент детерминации (R-квадрат). Желательно, чтобы этот коэффициент был не ниже 70-80%. Для обычной линейной регрессии с одним параметром можно просто возвести в квадрат коэффициент корреляции, чтобы его получить (отсюда и название  «R-квадрат»). 

**Коэффициент детерминации** – показатель качества регрессии, который равен доле вариации зависимой случайной величины, которую удалось объяснить с помощью регрессии.

Для оценки применимости регрессии к прогнозированию реальных данных, следует обратить внимание на следующие потенциальные проблемы:
- условная гетероскедастичность 
- автокорреляция 
- мультиколлинеарность 

**Условная гетероскедастичность** - зависимость ошибки регрессии от величины независимой величины (X).

<img src=pics/Getero.png>

**Автокорреляция** - когда ошибка регрессии зависит от предыдущих значений ошибки.

<img src=pics/CorAuto.png>

**Мультиколлинеарность** - когда две или более независимых величин (X) оказываются связаны (коррелированы) между собой.

### АНАЛИЗ ФИНАНСОВЫХ ВРЕМЕННЫХ РЯДОВ

**Анализ временных рядов** — совокупность математических методов анализа, предназначенных для прогнозирования временного ряда (значений случайной величины во времени).

Выделяют две группы методов, в зависимости от того, что используется в качестве зависимой переменной:
- трендовые модели (от времени);
- авторегрессионные модели (от прошлых значений величины).

**Трендовые модели** - изучают зависимость некоторой случайной величины от времени (например, зависимость процентной ставки от времени):

$$ y_t=\beta_0 + \beta_1(t) + \varepsilon_t $$

- t - порядковый номер периода времени
- $\beta_0$ и $\beta_1$ искомые коэффициенты трендовой модели

Авторегрессионные модели - изучают зависимость случайной величины от ее предыдущих значений:

$$x_t = \beta_0 + \beta_1x_{t-1} + \beta_1x_{t-2} +...+ \beta_px_{t-p} + \varepsilon_t $$

- $x_t$ текущее значение случайной величины- $x_t-1,\; x_t-2$, …  ее прошлые значения.

Применение авторегрессионных моделей в финансах - прогнозирование цен и доходностей акций, процентных ставок и волатильности финансовых активов

Практические проблемы метода:
- нестационарность - изменение свойств финансового временного ряда во времени, например, в связи с изменением государственного регулирования экономики, политической обстановки,  развития или стагнации рынка/отрасли и т.д.;
- сезонность - изменения параметров финансового временного ряда в связи с объективными экономическими циклами;
- условная гетероскедастичность - изменение волатильности случайной величины во времени (была рассмотрена выше).

### ПРИМЕРЫ ЗАДАЧ К РАЗДЕЛУ 5
[Задачи в экселе](05.Lecture/lec05.xlsx)