## Проект по анализу и предсказаниям временных рядов

Описание задачи:

На основе предоставленного датасета с историческими данными о заказах такси необходимо было провести первичный анализ данных и обучить модель которая будет прогнозировать спрос на следующий час

Используемые инструменты:

Для анализа были применены классические библиотеки в виде Pandas и Seaborn, так как Pandas предоставлял довольно удобные инструменты для работы с временными рядами и Seaborn позволял быстро отрисовывать удобные для восприятия графики. Из sklearn была применена кросс-валидация с параметром TimeSeriesSplit() и взято несколько простых моделей регрессии для прогнозирования спроса. Из сложных моделей был взят LGBM который и показал лучший результат.

Вывод:

Во время первичного анализа был замечен интересный тренд о том что спрос выше в воскресенье, понедельник и пятницу, а сильное падение во вторник и в субботу.
Для прогнозирования лучше всего подошёл алгоритм LGBM: он выдавал лучшее значение метрики с не очень высокими затратами времени.
