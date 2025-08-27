# Flight Delay Analysis (2000–2001)

## Project Overview
This project analyses a large dataset containing flight arrival and departure details for all commercial flights on major US carriers between 1987–2008.  
For this study, I focused on **2000–2001 data** to:
- Determine optimal travel times to minimise delays
- Assess the impact of aircraft age on delays
- Analyse passenger traffic between locations
- Detect cascading delays across airports
- Build models to predict flight delays

---

## Tools & Technologies
- **Languages:** Python, R  
- **Libraries:** Pandas, NumPy, Seaborn, Matplotlib, ggplot2  
- **Techniques:** Data Cleaning, EDA, Feature Engineering, Classification Models, Cascading Failure Analysis  

---

## Approach

### 1. Data Cleaning & Preparation
- Selected relevant columns (departure/arrival times, tail number, aircraft info)  
- Removed missing/irrelevant values (e.g., empty departure times)  
- Categorised departure times into four time periods (night, morning, afternoon, evening)  

### 2. Exploratory Data Analysis (EDA)
- Visualised delay distribution across time periods  
- Analysed whether older aircraft suffered more delays by merging flight & plane datasets  
- Mapped most popular routes and destinations using monthly flight counts  

### 3. Cascading Delay Analysis
- Defined cascading failures at flight/airport level:  
  - **Departure cascading:** dep delay (A) → arr delay (B) → dep delay (C)  
  - **Arrival cascading:** arr delay (A) → dep delay (B) → arr delay (C)  
- Compared cascading failures at major airports (e.g., Las Vegas vs Los Angeles)  

### 4. Predictive Modeling
- Created **total delay column** (dep + arr delay)  
- Classified delays into binary classes:  
  - Non-delay = ≤30 mins  
  - Delay = >30 mins  
- Built classification models: Logistic Regression, Random Forest, Gradient Boosting  

---

## Key Results & Insights
- **Best travel time:** Night flights (6pm–12am) had fewer delays  
- **Aircraft age:** No strong evidence older planes are more delay-prone  
- **Passenger traffic:** Certain hub routes dominated monthly flight counts  
- **Cascading failures:** Delays at major hubs triggered chain delays at connected airports  
- **Model performance:**  
  - Logistic Regression → **82.0% accuracy** (best performer)  
  - Random Forest → 81.6% accuracy  
  - Gradient Boosting → 81.7% accuracy  

---

## Visualisation

- Delay distribution by time of day  
  ![delay by time](https://github.com/syees/portfolio/blob/main/Programming%20for%20data%20science/Images/delay%20by%20time.png?raw=true)

