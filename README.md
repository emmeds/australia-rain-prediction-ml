# australia-rain-prediction-ml
#  Predizione Pioggia in Australia

## Panoramica
Questo progetto ha l'obiettivo di prevedere se pioverà domani in Australia basandosi su dati meteorologici storici.
Le sfide principali affrontate includono la gestione di dati sporchi e outlier, di classi sbilanciate, l'ottimizzazione avanzata di modelli di Machine Learning e il tuning della soglia decisionale.

##  Risultati Chiave
Dopo estesi test e ottimizzazioni, il modello migliore ha raggiunto i seguenti risultati:
- **Modello:** Random Forest (Ottimizzato con Ricerca Bayesiana)
- **AUC Score:** 0.864
- **Recall (Classe 1):** 78% (Miglioramento significativo rispetto alla baseline)
- **Soglia Ottimale:** 0.44 (Calcolata tramite l'Indice di Youden)

##  Tech Stack
- **Python** (Pandas, NumPy, Scikit-learn)
- **Ottimizzazione Bayesiana** (scikit-optimize)
- **Visualizzazione** (Matplotlib, Seaborn)

##  Metodologia
1. **Pulizia Dati:**
2. **Feature Engineering:** Trasformazione logaritmica per i dati di pioggia (skewed).
3. **Selezione Modello:** Confronto tra Naive Bayes, Decision Tree e Random Forest.
4. **Ottimizzazione:** Utilizzo di `BayesSearchCV` per il tuning degli iperparametri.
5. **Tuning della Soglia:** Regolazione della soglia decisionale utilizzando la statistica J di Youden per massimizzare il rilevamento della pioggia.
