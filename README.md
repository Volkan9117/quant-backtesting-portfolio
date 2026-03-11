# 📊 Python pour la Finance de Marché

> Portfolio de projets Python appliqués à la finance quantitative — analyse de données, indicateurs techniques, backtesting et Machine Learning.

---

## Présentation

Ce repository regroupe mes travaux en **Python appliqué à la finance de marché**, couvrant l'ensemble de la chaîne analytique : de la collecte et la préparation des données jusqu'à l'implémentation de modèles de Machine Learning intégrés dans des stratégies de trading.

Ces projets ont été réalisés dans le cadre de mon parcours autodidacte en finance quantitative, en vue d'un **Master Finance de Marché**. Ils illustrent ma capacité à manipuler des données financières réelles et à implémenter des concepts théoriques en code fonctionnel.

---

## Structure du repository

| Module | Thème | Compétences clés |
|--------|-------|-----------------|
| `01` | Préparation des données financières | `pandas`, `yfinance`, nettoyage, resampling |
| `02` | Rendements & Volatilité | Rendements simples/cumulés, volatilité annualisée |
| `03` | Moyennes mobiles (SMA & EMA) | `rolling()`, `ewm()`, visualisation interactive |
| `04` | Analyse technique | RSI, MACD, OBV, A/D Line, `plotly` |
| `05` | Backtesting | `backtrader`, stratégies SMA, Sharpe ratio, drawdown |
| `06` | Machine Learning en finance | Random Forest, classification, régression, signaux de trading |

---

## Détail des modules

### 01 — Préparation des données financières
Fondation de tout pipeline d'analyse quantitative : import depuis Yahoo Finance et CSV, nettoyage (valeurs manquantes, doublons, anomalies), gestion des séries temporelles et resampling (journalier → hebdomadaire → mensuel).

**Librairies :** `pandas`, `yfinance`, `numpy`

---

### 02 — Analyse des rendements et de la volatilité
Calcul et interprétation des métriques de performance fondamentales :
- Rendements journaliers simples : $R_t = \frac{P_t - P_{t-1}}{P_{t-1}}$
- Rendements cumulés : $RC_t = \prod_{i=1}^{t}(1 + R_i)$
- Volatilité annualisée : $\sigma_{annuelle} = \sigma_{journalière} \times \sqrt{252}$

**Librairies :** `pandas`, `matplotlib`, `seaborn`

---

### 03 — Maîtriser les moyennes mobiles (SMA & EMA)
Implémentation des deux principaux indicateurs de tendance :
- **SMA** (Simple Moving Average) via `rolling().mean()`
- **EMA** (Exponential Moving Average) via `ewm()`
- Visualisation interactive avec `plotly` et `ipywidgets`

**Librairies :** `pandas`, `numpy`, `matplotlib`, `plotly`, `ipywidgets`

---

### 04 — Analyse technique avancée
Implémentation des indicateurs techniques standards utilisés en salle des marchés :

| Indicateur | Usage |
|-----------|-------|
| **RSI** (Relative Strength Index) | Détection surachat / survente |
| **MACD** | Suivi de tendance et momentum |
| **OBV** (On-Balance Volume) | Pression acheteurs / vendeurs |
| **A/D Line** | Accumulation / distribution |

**Librairies :** `pandas`, `numpy`, `plotly`

---

### 05 — Backtesting de stratégies de trading
Simulation d'une stratégie de croisement de moyennes mobiles (SMA 20 / SMA 50) sur données historiques réelles :
- Implémentation avec `backtrader`
- Métriques de performance : rendement total, capital final, **drawdown maximal**, Sharpe ratio
- Analyse des biais courants (overfitting, frais de transaction)

**Librairies :** `backtrader`, `yfinance`, `matplotlib`, `pandas`

---

### 06 — Machine Learning appliqué à la finance
Deux approches ML appliquées à la prédiction boursière :

**Classification (Random Forest)**
- Prédiction signal achat/vente (0/1)
- Features : SMA, RSI et autres indicateurs techniques
- Métriques : accuracy, precision, recall, F1-score, AUC-ROC

**Régression (Random Forest Regressor)**
- Prédiction du prix de clôture J+1
- Métriques : RMSE, MAE, R²

**Intégration en stratégie de trading**
- Génération de signaux automatiques depuis les prédictions
- Comparaison avec une stratégie Buy & Hold

**Librairies :** `scikit-learn`, `pandas`, `numpy`, `matplotlib`

---

## Stack technique

```
Python 3.12
├── Data         → pandas, numpy, yfinance
├── Visualisation → matplotlib, seaborn, plotly
├── Finance      → backtrader
└── ML           → scikit-learn
```

---

## Installation & utilisation

```bash
# Cloner le repository
git clone https://github.com/votre-username/python-finance.git
cd python-finance

# Installer les dépendances
pip install -r requirements.txt

# Lancer un notebook
jupyter notebook
```

**`requirements.txt`**
```
pandas
numpy
yfinance
matplotlib
seaborn
plotly
ipywidgets
backtrader
scikit-learn
jupyter
```

---

## 📬 Contact

**Volkan ISLEYEN**
[LinkedIn]([https://linkedin.com/in/votre-profil](https://www.linkedin.com/in/volkan-isleyen-60584038a/)) · [Email](volkanisleyen86@gmail.com)

*Candidat Master Finance de Marché — Passionné de finance quantitative et de programmation Python*
