# Оценка маркетинговых компаний

### Задание
Маркетинг просит нас помочь с оценкой их рекламных компаний. Решено сделать это с помощью сегментации пользователей. 

Что необходимо получить: 

* визуализацию сегментации, обоснование границ сегментов
* портреты пользователей по самым интересным сегментам (пол, возраст)
* выводы, какие камании стоит продолжать, а какие закрыть  

Найти возможные аномалии в транзакциях

# Summary

### Сегментация

Сегментацию пользователей решено произвести RFM методом в разрезе по каждой рекламной кампании. Это позволяет проследить влияние кампании на пользователей по соотношения между сегментами, разделенными по степени вовлеченности пользователей. 

Сегменты: 

* Recency - как давно совершена крайняя покупка

1 - очень давно

2 - средне

3 - недавно

* Frequency - частота 

Посмотрим сколько в среднем в месяц пользователь совершает покупок

1 - мало

2 - средне

3 - много

* Monetary - сколько денег потратил клиент

1 - мало

2 - средне

3 - много

Разделение на сегменты символическое для того, чтобы показать методологию

Тепловая карта показывает какой процент пользователей, попавших под воздействие рекламной компании, отности к тому или иному RFM-сегменту. При необходимости более детального анализа лучше фильтровать непосредственно по рекламной кампании.

<img width="979" alt="Снимок экрана 2023-01-05 в 18 21 13" src="https://user-images.githubusercontent.com/113179175/210815319-4df341be-002c-4d29-878f-77e5b305e694.png">

По тепловой карте уже видно неудачные рекламые компании, направленные на возрастной сегмент 18-24.

Посмотрим немного детальнее на отдельные сегменты. Для примера возьмеем самый "лучший" 333 и самый "худший" 111. Для более детального анализа можно расширить число интересующих сегментов. 

<img width="940" alt="Снимок экрана 2023-01-05 в 18 28 20" src="https://user-images.githubusercontent.com/113179175/210816911-6d69aa84-b2fc-48d2-bc2b-7dbd43761449.png">

<img width="940" alt="Снимок экрана 2023-01-05 в 18 29 18" src="https://user-images.githubusercontent.com/113179175/210817194-c85b2a24-0ae6-4a4c-bdb8-4e01d18d4bd8.png">

Составим оценочную метрику (эффективность) - разницу между числом "желаемых" (активных, лояльных) пользователей (333) и "нежелаемых" (111) отнормированную на бюджет рекламной кампании. 

<img width="940" alt="Снимок экрана 2023-01-05 в 18 25 37" src="https://user-images.githubusercontent.com/113179175/210816393-568608a3-6577-4a91-ab18-8da5c0b4f899.png">

По графику уже можно определить, какие кампании оставить, а какие не стоит. Для того, чтобы понять какие из более успешных рекламных кампаний оставить, необходимо определиться с минимальным детектируем эффектом либо с минимальным профитом, который мы хотели бы извлечь.

### Ползователи 

Больше всего заказов оформляют женщиины и мужчны из возрастной группы 25-34 года. При этом больше всего денег приносят женщины из возрастных групп 25-34 и 35-44. Наивысший средний чек у женщин 35-44 и у мужчин 45-54.

<img width="940" alt="Снимок экрана 2023-01-13 в 12 49 53" src="https://user-images.githubusercontent.com/113179175/212290184-9a665231-c0cd-4a6e-a8ed-c63b990b5c9c.png">

<img width="940" alt="Снимок экрана 2023-01-13 в 12 50 17" src="https://user-images.githubusercontent.com/113179175/212290259-b38c9e37-00de-40db-ba0b-04a9763ea6d4.png">

<img width="940" alt="Снимок экрана 2023-01-13 в 12 50 40" src="https://user-images.githubusercontent.com/113179175/212290325-cf1e5b43-61e3-4ce9-b64a-4b8d574ee82a.png">

