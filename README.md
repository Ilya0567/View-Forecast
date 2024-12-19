# View-Forecast: VK Ads Auction Prediction

<h2>Команда № 33</h2>

* !["Богдан Танчук"](https://img.shields.io/badge/%D0%91%D0%BE%D0%B3%D0%B4%D0%B0%D0%BD-%D0%A2%D0%B0%D0%BD%D1%87%D1%83%D0%BA-blue)
* !["Илья Бецукели"](https://img.shields.io/badge/%D0%98%D0%BB%D1%8C%D1%8F-%D0%91%D0%B5%D1%86%D1%83%D0%BA%D0%B5%D0%BB%D0%B8-gold)
* !["Артемий Глобчастый"](https://img.shields.io/badge/%D0%90%D1%80%D1%82%D0%B5%D0%BC%D0%B8%D0%B9-%D0%93%D0%BB%D0%BE%D0%B1%D1%87%D0%B0%D1%81%D1%82%D1%8B%D0%B9-limegreen)
* !["Абдрахманов Антон"](https://img.shields.io/badge/%D0%90%D0%B1%D0%B4%D1%80%D0%B0%D1%85%D0%BC%D0%B0%D0%BD%D0%BE%D0%B2-%D0%90%D0%BD%D1%82%D0%BE%D0%BD-red)
* !["Георгий Килин"](https://img.shields.io/badge/%D0%93%D0%B5%D0%BE%D1%80%D0%B3%D0%B8%D0%B9-%D0%9A%D0%B8%D0%BB%D0%B8%D0%BD-orange)
<ul>
  <li><span style="background-color: blue; color: white; padding: 3px; border-radius: 5px;">Богдан Танчук</span></li>
  <li><span style="background-color: gold; color: black; padding: 3px; border-radius: 5px;">Илья Бецукели</span></li>
  <li><span style="background-color: limegreen; color: black; padding: 3px; border-radius: 5px;">Артемий Глобчастый</span></li>
  <li><span style="background-color: red; color: white; padding: 3px; border-radius: 5px;">Абдрахманов Антон</span></li>
  <li><span style="background-color: orange; color: black; padding: 3px; border-radius: 5px;">Георгий Килин</span></li>
</ul>


### [Презентация проекта](https://docs.google.com/presentation/d/1WLEXedNQ8Fe1tLqf7XRCUHHzyrKC_fTytUfvbkrmMg0/edit?usp=sharing)
### [Ноутбук с обработкой данных](https://colab.research.google.com/drive/1YXUPY6UTM2KXXmya9HeZQUq3HisU5-wo?usp=sharing)

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
4. Предсказания проверены на основе метрики **MSE** (Mean Squared Error), интерпретируемой как среднеквадратичная ошибка.

---





