# Разработка систем ИИ: распознавание (Scikit-learn)

Готовая практическая реализация к курсовой работе. Включает Jupyter Notebook, который:
- загружает данные (`sklearn.datasets.load_digits`),
- проводит предобработку,
- обучает **Logistic Regression**, **SVM (RBF)**, **Random Forest** с `GridSearchCV`,
- оценивает качество и рисует матрицы ошибок,
- сохраняет лучшие модели и сводку метрик.

## Быстрый старт (локально)
```bash
python -m venv .venv
source .venv/bin/activate  # Windows: .venv\Scripts\activate
pip install -r requirements.txt
jupyter notebook recognition_scikit_learn.ipynb
```

## Google Colab
1. Загрузите файл `recognition_scikit_learn.ipynb` в Colab (File → Upload notebook).
2. Запустите все ячейки. По умолчанию используется `load_digits`.
3. Чтобы включить MNIST (28x28), установите `USE_MNIST = True` в соответствующей ячейке.

## Результаты и артефакты
- Лучшие модели сохраняются в `artifacts/` (`best_LogReg.joblib`, `best_SVM_RBF.joblib`, `best_RF.joblib`).
- Матрицы ошибок — CSV-файлы `cm_*.csv`.
- Сводка метрик — `artifacts/summary.json`.

## Репозиторий
Загрузите все файлы на GitHub. Итоговую ссылку на репозиторий прикрепите преподавателю.
