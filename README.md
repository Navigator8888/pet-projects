# Проекты, выполненные самостоятельно


## Содержание

|Номер|Название проекта | Задачи проекта | Стек |
|:--| :--------------------- | :---------------------------------------------------------- |:-----------------|
|1| [Аналитический дашборд по вакансиям на сайтах поиска работы][1] | Индикаторы общего числа вакансий в базе, общего количества компаний-работодателей, список актуальных вакансий по специальностям, динамика количества вакансий, общее число джун-вакансий за последние 30 дней, за последнюю неделю, за вчера, за сегодня |Python, DataLens|
|2| [Исследование активности студентов в чатах мессенджера Slack][2]| Проанализировать поведение студентов в чатах, выявить паттерны, динамику, цикличность в течение дня, недели, месяца, года. Визуализировать свои находки. Понять, когда активность студентов в чатах наибольшая, и когда лучше публиковать посты. Проанализировать типы каналов, когорт, групп. Оценить в каких общения больше, в каких меньше, и как они различаются от когорты к когорте, от канала к каналу. | Python, Pandas, Matplotlib |
|3| [Анализ остатков, оборачиваемости и продаж на WB][3]| Компания, производитель профессиональной химии. Сбыт как через партнеров и дилеров, так и через маркетплейс Wildberries. Учет данных по производству и работе с дилерами ведется в 1С, данные по работе с маркетплейсами хранятся в базе данных Postgres. Цель - построение дашборда для кроссплатформенной аналитики остатков, продаж, оборачиваемости по всем источникам данных. | Python, SQL, DataLens |
|4| [Кластеризация клиентов методом KMeans][4]| Мы применяем методы обучения без учителя для группировки клиентов на основе их характеристик, таких как: годовой доход, оценка трат, возраст, годы работы с компанией и покупательское поведение. Сегментация клиентов может быть полезна для разработки маркетинговых стратегий, персонализации услуг и повышения лояльности клиентов. |Python, NumPy, Scikit-learn, Matplotlib и Seaborn|
|5| [Классификации изображений с использованием сверточных нейронных сетей][5]| В этом проекте решается задача классификации изображений с использованием сверточных нейронных сетей (CNN) на примере набора данных CIFAR-10, содержащего 60 000 цветных изображений размером 32x32 пикселя, распределенных по 10 классам, включая такие категории, как "самолет", "автомобиль", "кошка", "собака". Для решения задачи использованы библиотеки TensorFlow и Keras. |Python, TensorFlow, Keras, Matplotlib|
|6| [Прогнозирование доходов компании][6]| Этот проект демонстрирует применение методов машинного обучения для прогнозирования доходов компании на основе двух факторов: расходов на рекламу и зарплат сотрудников. Модель использует Ridge-регрессию с регуляризацией и полиномиальные признаки для повышения качества прогнозов и предотвращения переобучения. |Python, NumPy, Scikit-learn, Matplotlib|
|7| [Прогнозирование цен на жилье методом регрессии][7]| Этот проект о применении алгоритмов регрессии для решения задачи прогнозирования цен на жилье в зависимости от признаков - площадь и срок дома. Мы используем такие алгоритмы, как линейная регрессия, полиномиальная регрессия, Ridge и Lasso. Проект также включает стандартизацию данных, подбор гиперпараметров и визуализацию результатов. |Python, NumPy, Scikit-learn, Matplotlib|
|8| [Генеративная сеть для создания изображений цифр][8]| В этом проекте реализована Generative Adversarial Network (GAN), используемая для генерации изображений рукописных цифр из набора данных MNIST. Это демонстрация работы простого GAN, который обучается на наборе изображений и после завершения обучения способен генерировать реалистичные изображения цифр. |Python, NumPy, Scikit-learn, PyTorch, Matplotlib, Seaborn|
|9| [Моделирование ставок в аукционе при помощи теории игр][9]| Рассмотрим аукцион с несколькими участниками, где каждый делает ставку на лотерею. Используем модель аукциона с звкрытыми ставками, в которой участники делают ставки одновременно, не зная ставки других участников. Цель — проанализировать стратегию участников и их шансы на победу. |Python, Matplotlib, Seaborn|
|10| [Моделирование торгов на торговой площадке с использованием теории игр и алгоритмов машинного обучения][10]| Этот проект представляет собой моделирование торговых взаимодействий между покупателями и продавцами на торговой площадке с использованием теории игр и алгоритмов машинного обучения. Модель учитывает множество факторов, таких как стратегии участников, влияние внешних экономических условий, а также адаптацию ставок и цен с помощью Q-learning. Модель построена с учётом динамического взаимодействия участников, внешних факторов, а также стратегического поведения, зависящего от агрессивности или консервативности игроков. |Python, NumPy, Tensorflow, Matplotlib, Seaborn|
|11| [Стратегическое ценообразование в конкурентной среде с использованием теории игр][11]| Этот проект представляет модель стратегического ценообразования для нескольких компаний, используя подходы теории игр. Проект написан на языке Python и включает в себя простой симулятор взаимодействий компаний в конкурентной среде. Компании выбирают свои цены на основе текущего состояния рынка, стремясь максимизировать свою прибыль. |Python, NumPy, Matplotlib, Seaborn|
|12| [Моделирование военных конфликтов с помощью теории игр][12]| Используется упрощённая версия Q-обучения для определения оптимальных стратегий нескольких игроков (или сторон конфликта), которые могут изменять свои действия в зависимости от внешних факторов и успехов в предыдущих раундах. В проекте учитываются такие факторы, как динамическое взаимодействие, разрушение альянсов, учёт различных типов игроков (агрессивные, осторожные и сбалансированные), а также влияние внешней среды на матрицы выплат. |Python, NumPy, Matplotlib, Seaborn|
|13| [Модель маршрутизации трафика с учетом равновесия Уордаропа и машинного обучения][13]| Этот проект представляет собой симуляцию распределения трафика на дорожной сети с использованием теории игр и алгоритма Q-learning. Цель — продемонстрировать, как водители могут выбирать маршруты на основе разных факторов: время в пути, стоимость, комфорт и как распределение трафика может адаптироваться к различным внешним условиям - аварии, перекрытия дорог, пока система не достигнет состояния равновесия Уордаропа. |Python, NumPy, Matplotlib, Seaborn|
|14| [Поиск аномалий с использованием One-Class SVM, Isolation Forest и PCA][14]| Проект посвящён задаче обнаружения аномалий в данных с помощью методов машинного обучения. Мы рассмотрим три различных подхода: One-Class SVM, Isolation Forest и PCA. Проект включает как построение моделей, так и их визуализацию для наглядного отображения аномалий. |Python, NumPy, Matplotlib, Seaborn, Pyod|

[1]: https://clck.ru/357jw3
[2]: https://clck.ru/35rhvk
[3]: https://clck.ru/36G2SR
[4]: https://clck.ru/3E495h
[5]: https://clck.ru/3E49gm
[6]: https://clck.ru/3E4BAg
[7]: https://clck.ru/3E4BRG
[8]: https://clck.ru/3E4DyX
[9]: https://clck.ru/3E4FKo
[10]: https://clck.ru/3E4GSx
[11]: https://clck.ru/3E4Hs5
[12]: https://clck.ru/3E4K3v
[13]: https://clck.ru/3E4KFV
[14]: https://clck.ru/3E4q2S
