# ФИНАНСОВАЯ МАТЕМАТИКА
**Финансовая математика** – это основа всей современной теории экономики и финансов.

## 1. ВРЕМЕННАЯ СТОИМОСТЬ ДЕНЕГ

### КОНЦЕПЦИЯ ВРЕМЕННОЙ СТОИМОСТИ ДЕНЕГ

Сумма денежных средств, доступная в настоящий момент, имеют большую ценность (стоимость), чем эта же сумма в какой-то момент времени в будущем. Чем раньше мы получаем деньги, тем это выгоднее для нас!

### ПРОСТЫЕ И СЛОЖНЫЕ ПРОЦЕНТЫ

**Процентная ставка** – это количественное отражение временной стоимости денег, которая может интерпретироваться как:
- **Ставка доходности**, которую требует инвестор, чтобы вложить деньги в данную инвестицию
- **Альтернативная стоимость** (т.н. «вмененные издержки») – альтернативные возможности вложений для конкретного инвестора
- **Ставка дисконтирования** – это параметр, который используется для сравнения денежных сумм в разные моменты времени
Процентная ставка бывает двух видов:
- **Простая процентная ставка** – применяется только к основной сумме долга
- **Сложная процентная ставка** - учитывает начисление процентов на всю сумму, включая ранее начисленные проценты.



### ДИСКОНТИРОВАНИЕ И НАРАЩЕНИЕ

**i** - процентная ставка за один период

**n** - период выплат (каждый год)

**m** - периодичность, т.е. количество выплат в течении периода (внутри года)

**PV** (Present Value) - Текущая стоимость денег (В excel ПС() - приведенная стоимость)

**FV** (Future Value) - Будущая стоимость денег (В excel БС() - будущая стоимость)

**Дисконтирование** – процесс перевода денежной суммы от будущего момента времени к прошлому
<table border=1>
<tr><th>Простая процентная ставка</th><th>Сложная процентная ставка</th></tr>
<tr><td> 

$$PV=FV/(1+i*n)$$
</td><td>

$$PV=FV/((1+i)^n)$$
</td></tr>
</table>

**Наращение** - процесс перевода денежной суммы от прошлого момента к будущему
<table border=1>
<tr><th>Простая процентная ставка</th><th>Сложная процентная ставка</th></tr>
<tr><td> 

$$FV=PV*(1+i*n)$$
</td><td>

$$FV= PV*(1+i)^n$$
</td></tr>
</table>

**Выгоды максимально частой капитализации процентов** - в зависимости от условий начисления процентов при одной и той же процентной ставке эффект (то есть, итоговая сумма) будет различным!
<table border=1>
<tr><th>Наращение для начисления процентов по сложной ставке i в течении n периодов</th>
<th>Дисконтирование для начисления процентов по сложной ставке i в течении n периодов</th></tr>
<tr><td> 

$$FV=PV*(1 + i/m)^{n*m}$$
</td><td>

$$PV=FV*(1+i/m)^{n*m}$$
</td></tr>
</table>

**Эффективная процентная ставка** - та процентная ставка, которая дает тот же эффект с точки зрения итоговой денежной суммы, но при условии начисления 1 раз в год
$$FV = PV * (1 + эф.ставка)$$

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
$$(1 + Rном) = (1 + Rреал) * (1 + I)$$

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

### 1. ПРИМЕРЫ ЗАДАЧ
[Задачи в экселе](01.Lecture/lec01.xlsx)

## 2. РАСЧЕТОВ ПРОЦЕНТОВ

### ДЕНЕЖНЫЕ ПОТОКИ И АННУИТЕТЫ

**Денежный поток** – реальное движение денежных средств проекта в виде набора денежных сумм с привязкой к конкретным моментам времени. У каждой составляющей денежного потока есть три параметра: денежная сумма, момент времени и знак.

Если мы получаем деньги, то для нас эта сумма идет со знаком "+", если мы платим, то со знаком "-"

Для инвестиционных проектов: в начале идет т.н. **инвестиционная фаза**, когда нам приходится вкладывать деньги, а затем начинается **операционная фаза**, когда мы начинаем зарабатывать деньги.

Денежные потоки нерегулярны во времени. Но, часто, мы имеем дело с т.н. аннуитетом

**Аннуитет** - денежный поток, элементы которого равны между собой и поступают или уплачиваются через равные промежутки времени
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

$PV=A*\frac{1-(1+r)^{-n}}{r}$

$FV=A*\frac{(1+r)^n-1}{r}$

#### Аннуитет пренумерандо 

$PV=A*\frac{1-(1+r)^{-n}}{r}*(1+r)$

$FV=A*\frac{(1+r)^n-1}{r}*(1+r)$

#### Перпетуитет

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

### 2. ПРИМЕРЫ ЗАДАЧ
[Задачи в экселе](02.Lecture/lec02.xlsx)