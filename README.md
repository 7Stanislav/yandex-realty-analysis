# 🏠 Real Estate Listings Data Analysis (Yandex.Realty) / Исследование объявлений о продаже квартир (Яндекс.Недвижимость)

## Project Overview / Обзор проекта
**EN:**  
This project is an exploratory data analysis (EDA) of apartment listings in Saint Petersburg and nearby localities.  
The goal is to determine the market value of real estate by identifying key parameters influencing price.  
The results can be used as a foundation for building an automated system to detect anomalies and potential fraud in the housing market.  

**RU:**  
Данный проект представляет собой исследовательский анализ данных (EDA) объявлений о продаже квартир в Санкт-Петербурге и соседних населённых пунктах.  
Цель проекта — определить рыночную стоимость объектов недвижимости путем выявления основных параметров, влияющих на цену.  
Полученные результаты могут быть использованы для построения автоматизированной системы, способной отслеживать аномалии и потенциальную мошенническую деятельность на рынке недвижимости.  

---

## Tasks / Задачи проекта
**EN:**  
- **Data preprocessing:** handle missing values, duplicates, adjust data types  
- **Feature engineering:**  
  - price per square meter  
  - day of week, month, year of listing  
  - floor type (first, last, other)  
  - distance to city center (km)  
- **Exploratory Data Analysis (EDA):**  
  - analyze key property parameters (area, price, rooms, ceiling height, floor type, etc.)  
  - build histograms & scatter plots  
  - identify factors affecting apartment prices  
  - calculate average price per square meter in top-10 most popular locations  
  - analyze effect of distance to Saint Petersburg city center on price  
- **Conclusions:** summarize insights and recommendations  

**RU:**  
- **Предобработка данных:** обработка пропусков, дубликатов, корректировка типов данных  
- **Добавление новых параметров:**  
  - цена квадратного метра  
  - день недели, месяц, год публикации  
  - тип этажа (первый, последний, другой)  
  - расстояние до центра в км  
- **EDA (исследовательский анализ):**  
  - анализ площади, цены, комнат, высоты потолков, этажа  
  - построение гистограмм и scatter-графиков  
  - выявление факторов, влияющих на стоимость  
  - расчет средней цены м² в 10 самых популярных локациях  
  - исследование зависимости цены от расстояния до центра СПб  
- **Выводы:** формулирование ключевых результатов  

---

## Data Source / Источник данных
**EN:**  
The dataset was provided by *Yandex.Realty* and contains several years of apartment listing history.  
It includes user-entered fields (price, area, number of rooms, etc.) and automatically generated GIS data (distance to city center, nearest airport, number of parks, ponds, etc.).  

File: `real_estate_data.csv`  

**RU:**  
Данные предоставлены сервисом *Яндекс.Недвижимость* и представляют собой архив объявлений о продаже квартир за несколько лет.  
Каждый объект содержит данные, введенные пользователем, а также автоматически полученные картографические параметры (расстояние до центра, до аэропорта, число парков и водоёмов и др.).  

Файл: `real_estate_data.csv`  

---

## Libraries / Используемые библиотеки
- pandas — data manipulation & analysis  
- numpy — numerical computations  
- matplotlib — visualization  
- seaborn — statistical graphics  
- scipy.stats — statistical tests  
- IPython.display — notebook display utilities  

---

## Research Workflow / Ход исследования
**EN:**  
1. **Load & initial review** — inspect head, data types, info  
2. **Data preprocessing** —  
   - handle missing values (ceiling_height, balcony, kitchen_area, etc.)  
   - adjust data types for optimization  
   - fix duplicates in locality names  
3. **Feature engineering** —  
   - calculate price per square meter  
   - extract day, month, year of listing  
   - classify floor type (first, last, other)  
   - convert distance to center into kilometers  
4. **EDA** —  
   - analyze distribution of area, price, rooms, ceiling height, days on market  
   - visualize with histograms and scatter plots  
   - correlation analysis with price  
   - average price per m² in top-10 localities  
   - effect of distance to Saint Petersburg center  
5. **Conclusions** — summarize key results  

**RU:**  
1. **Загрузка и обзор** — изучение первых строк, типов, информации о данных  
2. **Предобработка** —  
   - обработка пропусков (ceiling_height, balcony, kitchen_area и др.)  
   - изменение типов данных  
   - устранение дублей в названиях населённых пунктов  
3. **Фичеринга** —  
   - расчет цены м²  
   - извлечение дня, месяца, года публикации  
   - определение типа этажа  
   - перевод расстояния до центра в километры  
4. **EDA** —  
   - анализ площади, цены, комнат, этажности, времени экспозиции  
   - визуализации распределений  
   - корреляции цены с параметрами  
   - средняя цена м² в топ-10 локациях  
   - исследование влияния расстояния до центра  
5. **Общие выводы** — суммирование результатов  

---

## How to Run / Как запустить проект
**EN:**  
1. Clone repository:  
   ```
   git clone https://github.com/7Stanislav/real-estate-analysis
   ```  
2. Install dependencies:  
   ```
   pip install pandas numpy matplotlib seaborn scipy
   ```  
3. Place `real_estate_data.csv` in the project directory.  
4. Open `project.ipynb` in Jupyter Notebook/Lab.  
5. Run all cells.  

**RU:**  
1. Клонируйте репозиторий:  
   ```
   git clone https://github.com/7Stanislav/real-estate-analysis
   ```  
2. Установите зависимости:  
   ```
   pip install pandas numpy matplotlib seaborn scipy
   ```  
3. Поместите `real_estate_data.csv` в папку проекта.  
4. Откройте `project.ipynb` в Jupyter Notebook или JupyterLab.  
5. Запустите все ячейки по порядку.  
