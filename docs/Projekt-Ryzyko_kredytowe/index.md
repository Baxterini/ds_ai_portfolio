# 🏦 Ryzyko kredytowe – perspektywa biznesowa

Kompletny projekt analityczno-modelowy z obszaru *Credit Risk*, pokazujący jak z danych historycznych zbudować produkcyjny pipeline machine learning wspierający decyzje kredytowe w instytucji finansowej.

Celem projektu jest estymacja prawdopodobieństwa niespłacenia zobowiązania przez klienta (default) oraz zaprezentowanie całego cyklu życia rozwiązania ML:
od eksploracji danych, przez inżynierię cech i modelowanie, aż po walidację i warstwę interpretowalności opartą o SHAP.

Model oparty na XGBoost osiąga wysoką zdolność separacji klientów niskiego i wysokiego ryzyka (ROC-AUC ≈ 0.80) i pozwala świadomie zarządzać kompromisem pomiędzy bezpieczeństwem finansowym a dostępnością kredytu.

---
## Linki

- 📂 Repozytorium: https://github.com/Baxterini/EDA_ML_Bank  
- 📄 Raport PDF: [Pobierz](link-do-pdf-w-repo)  
- 🧪 Notebook główny: `Credit_Risk_Case_Study.ipynb`



## 📁 Struktura projektu

| Plik / katalog | Opis |
|----------------|------|
| `01_EDA_bank.ipynb` | Eksploracyjna analiza danych (EDA) |
| `02_Feature_Engineering_and_Modeling.ipynb` | Przygotowanie cech i pierwsze modele |
| `03_Bank_Baseline_Model_(XGBoost_Pipeline).ipynb` | Pipeline bazowy z XGBoost |
| `04_Model_Comparison_and_Optimization.ipynb` | Porównanie modeli i tuning |
| `05_Explainability_SHAP.ipynb` | Interpretowalność modeli (SHAP) |
| `Credit_Risk_Case_Study.ipynb` | Spójna wersja raportowa projektu |
| `credit_risk_case_study.html` | Raport w formie HTML |
| `credit_risk_case_study_PDF.pdf` | Raport w formie PDF |
| `docs/img/` | Wykresy i grafiki do dokumentacji |

---

## 🔍 Zakres projektu

- analiza struktury danych i problemu biznesowego  
- eksploracja rozkładów i zależności cech  
- inżynieria cech (feature engineering)  
- budowa pipeline’u ML (scikit-learn + XGBoost)  
- walidacja modeli (ROC, PR, confusion matrix)  
- tuning hiperparametrów  
- porównanie wariantów modeli  
- warstwa explainability (SHAP: global + lokalna interpretacja)  
- raport biznesowy w formie PDF / HTML  

---

## 📊 Wartość biznesowa

Projekt pokazuje, jak:

- przełożyć dane historyczne na realne decyzje kredytowe,  
- zarządzać kosztem fałszywie pozytywnych i negatywnych decyzji,  
- budować modele zgodne z wymogami audytowalności,  
- uzasadniać pojedyncze predykcje w sposób zrozumiały dla analityka i regulatora.

To przykład, jak model ML staje się narzędziem wspierającym decyzje biznesowe, a nie tylko algorytmem „black box”.

---

## 🛠 Technologie

- Python  
- pandas, numpy  
- scikit-learn  
- XGBoost  
- SHAP  
- matplotlib / seaborn  
- Jupyter Notebook  

---

## Wizualizacje z projektu

![Rozkład klas – default](img/default_distribution.png)

*Problem biznesowy: dane są niezbalansowane – ponad 1/3 klientów to przypadki wysokiego ryzyka.*

![Porównanie modeli](img/model_comparison.png)

*Model po tuningu znacząco poprawia zdolność separacji klientów.*

![SHAP – wpływ cech](img/shap_summary.png)

*Explainability: widać, które cechy najbardziej wpływają na decyzję modelu.*


---

Autor: Rafał Król  
