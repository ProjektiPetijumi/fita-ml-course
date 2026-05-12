# Predict Students' Dropout and Academic Success

## Problēma
Prognozējam, vai students absolvēs, pamet studijas vai turpina studēt, 
izmantojot akadēmiskos un demogrāfiskos datus. Agrīna dropout prognozēšana 
ļauj augstskolām savlaicīgi iejaukties un palīdzēt riska studentiem.

## Datasets
- Avots: [UCI ML Repository](https://archive.ics.uci.edu/dataset/697/predict+students+dropout+and+academic+success)
- Izmērs: 4424 rindas × 37 kolonnas
- Target kolonna: Target (Dropout / Enrolled / Graduate)

## Pieeja
- ML tips: Klasifikācija (3 klases)
- Pipeline: StandardScaler → GradientBoostingClassifier
- Feature Engineering: Approval_rate, Total_approved, Avg_grade
- Optimizācija: GridSearchCV (cv=5)

## Rezultāti
- Bāzes modelis (Logistic Regression): F1 = 0.748
- Random Forest: F1 = 0.766
- Labākais modelis (Gradient Boosting): F1 = 0.775
- Galvenā pazīme: Approval_rate (kursu nokārtošanas līmenis)

## Faili
- `week4_homework.ipynb` — galvenais notebook
- `data.csv` — datasets
- `week1_homework.ipynb` — W1: Klasifikācija (F1=0.628)
- `week2-1_homework.ipynb` — W2: Regresija (R²=0.046)
- `week3_homework.ipynb` — W3: Klasterizācija + Validācija (CV F1=0.633)

## Kā palaist
1. Lejupielādē repozitoriju
2. Atver `week4_homework.ipynb` Jupyter Notebook
3. Izpildi visas šūnas (Kernel → Restart & Run All)

## Autore
Ilona | FITA ML kurss | 2026. gada maijs
