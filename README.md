# TestWorkGreyloud
Simple HTML
Прекондишен:

Создать новый проект на GitHub (по окончанию задания отправить линк на него). Обязательным условием является использование css препроцессора и организация сборки проекта с использованием gulp для development и production.

Задание:

Необходимо сверстать отзывчивую (responsive) страницу без использования javascript.

Страница занимает 100% высоты окна браузера, тянется до 1920px и содержит:

1. свободные области (синего цвета)
- сверху (там обычно живет главное меню, высота фикс)
- слева (для дополнительного вертикального меню, ширина фикс)
- снизу (мало ли понадобится, высота фикс)
- справа (минимальная ширина 4px, максимум не ограничен)

Все свободные области, кроме правой, можно выполнить отступами.
Правая должна быть элементом (чтобы, при необходимости, в него что-то вставить можно было)

2. кнопки в верхней части страницы

3. три колонки. У каждой колонки есть свой хедер и футер.
- левая. Имеет два состояния: свернутое (80px) и развернутое (240px).
- средняя  — контентная область. Минимальная ширина 720px.
- правая. Имеет минимальную (300px) и максимальную (600px) ширину.

Скролирование в колонках должно быть доступно в области между хедером и футером, если не указано иное поведение.

Левая колонка дополнительно содержит однотипные плашки с фотографией (изображена в виде серого круга) и именем.
Скролирование должно происходить под первую плашку. Область скрола отмечена фиолетовой рамкой (scroll-area.png)
По наведению на левую колонку, в свернутом состоянии, она должна отображаться в развернутом состоянии поверх средней колонки.

Принцип работы.
Если места достаточно, левая колонка отображается в развернутом виде, правая имеет максимальную ширину, средняя занимает все остальное место (layout-max.png)
При уменьшении ширины окна браузера:
1. уменьшается свободная область справа до минимальной ширины
2. уменьшается ширина средней колонки
3. при достижении ширины браузера 1520px левая колонка переходит в свернутое состояние
4. при достижении средней колонки минимальной ширины уменьшается ширина правой колонки
5. после достижения правой колонкой минимальной ширины (layout-large.png) и дальнейшем уменьшении ширины окна, колонка скрывается (layout-min.png)
При увеличении ширины браузера последовательность обратная.
