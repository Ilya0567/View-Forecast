# View-Forecast: VK Ads Auction Prediction

### Описание задачи

Проект посвящен прогнозированию количества просмотров рекламных объявлений ВКонтакте. Основная задача — предсказать, сколько пользователей увидят объявление в будущем, используя исторические данные о показах, демографию пользователей и параметры кампаний.

---

### Доступные данные

1. **`users.tsv`**: данные о пользователях (ID, пол, возраст, город).
2. **`history.tsv`**: история показов рекламы (час, ставка CPM, площадка, пользователь).
3. **`validate.tsv`**: объявления для валидации (ставка CPM, время запуска и остановки, площадки, аудитория).
4. **`validate_answers.tsv`**: эталонные ответы (доли пользователей, увидевших объявление один, два или три раза).

---

### Подход к решению

1. Проведена предварительная обработка и анализ данных.
2. Опробованы основные модели из классического ML (линейные модели, решающие деревья и ансамбли).
3. Наилучшие результаты показали:
   - **XGBoost** и **GRU** с метрикой **MSE**.
4. Предсказания проверены на основе метрики **Smoothed Mean Log Accuracy Ratio**, интерпретируемой как среднее относительное расхождение.

---

### Запуск проекта

1. Установите зависимости: `pandas`, `numpy`, `xgboost`, `tensorflow` (для GRU).
2. Загрузите исходные файлы данных.
3. Запустите скрипт анализа:

   ```bash
   python main.py




