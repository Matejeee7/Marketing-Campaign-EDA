# 🛒 Analiza Kupovnih Navika – Marketing Campaign EDA  
### *(Croatian / English – bilingual README)*

---

# 🇭🇷 1. Uvod (HR)

Ovaj projekt predstavlja detaljnu eksplorativnu analizu (EDA) marketinške kampanje koristeći Python i podatke o 2.240 kupaca. Analiziraju se:

- demografske karakteristike kupaca  
- prihodi i obiteljske navike  
- potrošnja u 6 kategorija proizvoda  
- navike kupnje (store, web, katalog)  
- uspješnost marketinških kampanja  

**Cilj:** razumjeti obrasce ponašanja kupaca, segmentirati ih te izvući poslovne uvide koji mogu pomoći u optimizaciji marketinških strategija.

---

# 🇬🇧 1. Introduction (EN)

This project provides an in-depth Exploratory Data Analysis (EDA) of a marketing campaign dataset containing information on 2,240 customers. The analysis covers:

- demographic attributes  
- income and family structure  
- spending across six product categories  
- purchasing behavior (store, web, catalog)  
- marketing campaign responses  

**Goal:** understand customer behavior patterns, perform segmentation, and extract business insights that can support marketing optimization.

---

# 🇭🇷 2. Priprema i čišćenje podataka (HR)

Uočen je mali broj nepravilnosti koje su ispravljene:

- 24 *Income* null vrijednosti popunjene median vrijednošću  
- uklonjen ekstremni outlier `Income = 666666`  
- `Dt_Customer` pretvoren u *datetime*  
- kreirana nova varijabla `Children = Kidhome + Teenhome`  
- kreiran novi feature `Total_Spending` (ukupna potrošnja kupca)

---

# 🇬🇧 2. Data Cleaning & Preparation (EN)

The dataset required several cleaning steps:

- 24 missing values in *Income* filled using the median  
- removed one extreme outlier (`Income = 666666`)  
- converted `Dt_Customer` to datetime  
- created `Children = Kidhome + Teenhome`  
- added new feature `Total_Spending` (sum of all spending categories)

---

# 🇭🇷 3. Analiza (HR)

### 🔹 Distribucije  
- Prihodi su blago desno-skewed  
- Većina kupaca troši malo, dok mali broj troši vrlo puno (Pareto efekt)

### 🔹 Korelacije  
Najveći doprinos ukupnoj potrošnji imaju:  
- **Vino (0.89)**  
- **Mesni proizvodi (0.84)**  
Jasna skupina kupaca visokih vrijednosti.

### 🔹 Segmentacija kupaca  
- Kupci **bez djece** troše najviše  
- Najveći potrošači su u **High Income** grupi  
- Najpopularniji kanal: **Store**, zatim **Web**, najmanje **Catalog**

---

# 🇬🇧 3. Analysis (EN)

### 🔹 Distributions  
- Income is slightly right-skewed  
- Spending follows a strong Pareto pattern (small group of high spenders)

### 🔹 Correlations  
Strongest contributors to total spending:  
- **Wine (0.89)**  
- **Meat Products (0.84)**  

Clear presence of high-value customer clusters.

### 🔹 Customer Segmentation  
- Customers **without children** spend the most  
- **High-income** group dominates in total spending  
- Most purchases occur in **Store**, followed by **Web**, then **Catalog**

---

# 🇭🇷 4. Poslovni uvidi (HR)

1. Kupci bez djece i kupci s visokim prihodima generiraju najveći dio prihoda.  
2. Premium kategorije (vino, meso) najviše utječu na ukupnu potrošnju.  
3. Store kanal je dominantan, no Web kanal ima najveći potencijal rasta.  
4. Jasni segmenti potrošača omogućuju preciznije targetiranje i personalizaciju.  
5. Pareto efekt: fokusirati kampanje na top 20% kupaca.

---

# 🇬🇧 4. Business Insights (EN)

1. High-income and child-free customers generate the majority of revenue.  
2. Premium categories (wine, meat) drive total spending the most.  
3. Store channel is dominant, while the Web channel shows strong growth potential.  
4. Clear customer segments enable precise targeting and personalization.  
5. Pareto effect: focus campaigns on the top-spending 20% of customers.

---

# 🇭🇷 5. Vizualizacije (HR)

Projekt uključuje:  
- histplot i boxplot distribucija  
- scatterplot (Income vs Spending)  
- korelacijske heatmape  
- segmentacijske grafove  
- analizu kupovnih kanala  

---

# 🇬🇧 5. Visualizations (EN)

Project includes:  
- distribution plots (histogram, boxplot)  
- scatterplot (Income vs Spending)  
- correlation heatmap  
- segmentation visualizations  
- purchase channel analysis  

---

# 🇭🇷 6. Zaključak (HR)

Projekt pokazuje kako jednostavnom EDA analizom možemo dobiti duboke uvidi u ponašanje kupaca te izgraditi temelje za marketinške modele i preporuke.

---

# 🇬🇧 6. Conclusion (EN)

This project demonstrates how EDA can uncover meaningful customer behavior patterns and support data-driven marketing strategies.

---

# 📂 🇭🇷 Struktura repozitorija / 🇬🇧 Repository Structure

/data
marketing_campaign.csv
/notebooks
marketing_campaign_eda.ipynb
/images
(graph .png files)
README.md


---

# 🇭🇷 7. Korištene tehnologije (HR)  
# 🇬🇧 7. Technologies Used (EN)

- Python  
- Pandas  
- NumPy  
- Seaborn  
- Matplotlib  
- Google Colab
