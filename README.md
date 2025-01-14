# AutoML

# Исследование методов AutoML для оптимизации параметров нейронных сетей в задачах компьютерного зрения

Этот проект посвящён исследованию методов автоматического машинного обучения (AutoML) для настройки гиперпараметров и архитектуры моделей в задачах классификации изображений. В ходе работы изучены AutoML фреймворки, такие как AutoKeras и H2O AutoML, и их применение к набору данных Flowers Dataset.

## Описание проекта

Проект исследует:
- Автоматическую настройку нейронных сетей с использованием AutoML.
- Сравнение AutoML подходов с вручную настроенной моделью.
- Зависимость точности моделей от времени обучения.
- Эффективность ансамблирования и NAS в задачах классификации.

## Используемые технологии

- **Языки**: Python
- **Библиотеки**: TensorFlow, AutoKeras, H2O AutoML, OpenCV, NumPy, Matplotlib
- **Фреймворки AutoML**: AutoKeras, H2O AutoML

## Установка

1. Убедитесь, что у вас есть доступ к Google Colab.
2. Установите необходимые зависимости, запустив ячейки кода в Colab.

## Запуск

1. Ссылка на блокнот [Google Colab Notebook](https://colab.research.google.com/drive/1SKAdM02d8kCeWMcNEvFdTm3RRahIbCjB?usp=sharing).  
2. Подготовьте набор данных:
   - Загрузите [Flowers Dataset](https://www.kaggle.com/datasets/imsparsh/flowers-dataset).
   - Разместите данные в папке `data/` на вашем Google Drive.
3. Следуйте инструкциям в ноутбуке для выполнения всех этапов исследования.

## Структура репозитория

- `notebooks/` — Основной Jupyter Notebook для проекта.
- `data/` — Данные набора Flowers Dataset.
- `results/` — Сохранённые модели и результаты экспериментов.

## Результаты

| Модель         | Точность | Время обучения |
|----------------|----------|----------------|
| CNN (ручная)   | 75%      | 90 минут       |
| AutoKeras      | 82%      | 60 минут       |
| H2O AutoML     | 78%      | 60 минут       |

## Выводы

AutoML фреймворки продемонстрировали высокую эффективность по сравнению с ручной настройкой. AutoKeras показал лучшие результаты благодаря NAS, в то время как H2O AutoML отличился гибкостью и удобством.
