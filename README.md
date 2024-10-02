# Streamlit Iris Demo

Цей проєкт демонструє, як розгорнути модель машинного навчання за допомогою Streamlit для класифікації квітів ірису на три види: `setosa`, `versicolor` та `virginica`. Додаток дозволяє користувачам вводити характеристики квітки та отримувати прогноз на основі навченої моделі Random Forest.

Протестувати роботу аплікейшену можна за посиланням: https://app-iris-demo-xqcnetfwfjao3nnv3jelc3.streamlit.app/
Якщо за посиланням виводиться повідомлення "This app has gone to sleep due to inactivity. Would you like to wake it back up?" просто натисніть кнопку "Yes, get this app back up!" і зачекайте півхвилини.

## Структура проєкту

- **data/**: Директорія, що містить набір даних Iris (`iris.csv`).
- **images/**: Директорія для зберігання зображень, які використовуються в додатку.
- **models/**: Директорія, що містить навчену ML-модель.
- **app.py**: Основний файл застосунку Streamlit.
- **requirements.txt**: Список необхідних Python-пакетів.
- **train.ipynb**: Jupyter Notebook для навчання моделі Random Forest.

## Налаштування

### Передумови

Переконайтеся, що у вас встановлений Python 3.12 або новішої версії. Також потрібно встановити необхідні пакети, зазначені в `requirements.txt`.

### Встановлення

1. **Клонуйте репозиторій**:
   ```bash
   git clone https://github.com/your-username/streamlit-iris-demo.git
   cd streamlit-iris-demo
   ```

2. **Створіть віртуальне середовище** (необов'язково, але рекомендовано):
   ```bash
   python -m venv venv
   source venv/bin/activate   # На Windows використовуйте `venv\Scripts\activate`
   ```

3. **Встановіть необхідні пакети**:
   ```bash
   pip install -r requirements.txt
   ```

### Навчання моделі

Щоб навчити класифікатор Random Forest, запустіть Jupyter Notebook `train.ipynb`:

1. Відкрийте Jupyter Notebook `train.ipynb`.

2. Виконайте кроки, описані в notebook, щоб навчити модель та зберегти її в директорії `models/`.

### Запуск додатку Streamlit

Запустіть додаток Streamlit локально за допомогою наступної команди:

```bash
streamlit run app.py
```

Додаток буде доступний за адресою `http://localhost:8501`.
