## Определение произрастающей с/х культуры - Agro Data Science Cup
**Задача:** Определить сельскохозяйственную культуру по ежедневным значениям нормализованного индекса вегетации.

**Решение:**
1. Для уменьшения размерности взяла средние данные по каждому месяцу.
2. Обучащая и тестовая выборка отличались, поэтому добавила новые признаки и оставила те, которые позволяют уменьшить различие между выборками, при этом не сильно вляли на предсказательную способность модели.
3. Т.к. метрикой была f1-weighted и больший вес имело правильное определение культуры у больших классов, было принято решение убрать из обучающей выборки редкие классы (где менее 7 объектов класса).
