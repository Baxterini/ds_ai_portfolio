# 🏦 Bank Churn Prediction (SHAP) – Explainable AI w praktyce

## 🔗 Repozytorium GitHub

Pełny kod aplikacji znajdziesz tutaj:  
👉 **[GitHub Repo](https://github.com/Baxterini/churn-prediction-shap)**  
👉 **[Live demo](https://churn-prediction-shap.streamlit.app/)**
---
![Widok główny aplikacji](/img/churn_1.png)
![Wyjaśnienie predykcji SHAP](/img/churn_2.png)
![Dane klienta](/img/churn_3.png)


Churn (odejście klienta) to jeden z kluczowych problemów w sektorze bankowym i usługowym.  
Utrzymanie klienta bywa tańsze niż pozyskanie nowego, a szybka reakcja może realnie ograniczyć straty.

Ten projekt pokazuje, jak połączyć **predykcję ML** z **wyjaśnialnością (Explainable AI)**, aby model nie był „czarną skrzynką”, lecz narzędziem wspierającym decyzje biznesowe.

---

## 🔍 Co potrafi aplikacja?

- Przewiduje **ryzyko churnu** dla wybranego klienta (prawdopodobieństwo).
- Pozwala zmieniać **próg decyzyjny (threshold)**, dopasowując czułość modelu do potrzeb biznesu.
- Wyjaśnia decyzję modelu dla konkretnego klienta przy pomocy **SHAP waterfall** (lokalne wyjaśnienie).
- Udostępnia podgląd **surowych cech klienta** wraz z czytelnym **słowniczkiem zmiennych**.
- Obsługuje opisy i interpretacje w **języku polskim i angielskim (PL / EN)**.

---

## 🧠 Dlaczego to ważne?

W praktyce biznesowej sama predykcja to za mało — kluczowe jest pytanie:  
**„dlaczego model podjął taką decyzję?”**

Aplikacja pomaga:
- zrozumieć czynniki zwiększające i zmniejszające ryzyko churnu,
- budować zaufanie do modelu wśród osób nietechnicznych,
- podejmować świadome decyzje retencyjne (np. dobór ofert, kontakt z klientem),
- jasno rozróżniać **prawdopodobieństwo** od **finalnej decyzji** (próg).

---

## 🧰 Technologie użyte w projekcie

- **Streamlit** – interaktywny interfejs webowy  
- **Python / pandas / numpy** – przetwarzanie danych  
- **scikit-learn** – preprocessing i pipeline  
- **XGBoost** – model predykcyjny  
- **SHAP** – wyjaśnialność i wykresy waterfall  
- **matplotlib** – wizualizacje w aplikacji  

---

## 🎯 Cel projektu

Celem projektu jest pokazanie, że predykcja churnu może być nie tylko skuteczna, ale też **zrozumiała i użyteczna biznesowo**.

To przykład aplikacji ML:
- z czytelnym interfejsem,
- kontrolą progu decyzyjnego,
- lokalnym wyjaśnieniem predykcji dla pojedynczego klienta,
- gotowej do wykorzystania jako demo lub punkt wyjścia do realnych wdrożeń.
