
# Analyse von Olist – einem brasilianischen Online-Marktplatz 🚀

Eine datengetriebene Untersuchung des Olist-Datensatzes. Ziel ist es, aus den vorhandenen Daten relevante Handlungsempfehlungen abzuleiten, die zur Optimierung des Geschäfts beitragen können.

## 📊 Projektübersicht

**Problemstellung:** 
Olist ist ein brasilianischer Online-Marktplatz, auf dem viele unterschiedliche Händler ihre Produkte anbieten. Der Datensatz enthält detaillierte Informationen zu Bestellungen, Umsätzen, Kunden, Bewertungen und Lieferungen. Für datengetriebene Entscheidungen im E-Commerce ist es entscheidend, sowohl die grundlegenden Geschäftszahlen als auch tiefergehende Einflussfaktoren zu verstehen.

**Ziel:** 
Zentrale Muster im Geschäftsbetrieb von Olist identifizieren und daraus Handlungsempfehlungen für die Optimierung des Geschäfts ableiten.

**Methoden:** 
-Explorative Datenanalyse (EDA) der Transaktionsdaten
-Datenbereinigung, um Konsistenz sicherzustellen
-Deskriptive Analysen und Visualisierungen
-Hypothesengetriebene Untersuchungen zu Zusammenhängen in den Daten

## 🎯 Key Findings

<!-- Hier deine wichtigsten Erkenntnisse in 3-5 Bullet Points -->
- 📈 **Erkenntnis 1:** Kurze Beschreibung
- 🔍 **Erkenntnis 2:** Kurze Beschreibung  
- 💡 **Erkenntnis 3:** Kurze Beschreibung

## 📁 Repository Struktur

```
├── data/
│   ├── raw/                    # Originaldaten
│   └── processed/              # Bereinigte Daten
├── notebooks/                  # Jupyter Notebooks
│   └── 01_exploration.ipynb    # Datenexploration
├── src/dpp                     # Python Module
├── test/                       # Unit Tests
├── pyproject.toml              # Projektkonfiguration
└── docs/                       # Zusätzliche Dokumentation
```

## 🔧 Verwendete Technologien

**Programmiersprachen:**

Python

**Libraries & Frameworks:**
pandas, numpy, matplotlib, seaborn, scikit-learn (für logistische Regression), pathlib (Dateiverwaltung)

**Tools:**
VS Code, Jupyter Notebooks, Git & GitHub, uv (Python-Paketmanager)

## 📊 Daten

**Datenquelle:** 
Olist Brazilian E-Commerce Dataset
— Datensammlung eines brasilianischen Online-Marktplatzes (Olist).

**Datensatz-Größe:** 
8 verknüpfte CSV-Dateien
ca. 100 000 Bestellungen
über 3 000 Seller
über 32 000 Produkte
rund 500 MB Rohdaten

**Wichtige Features:** 
order_purchase_timestamp – Zeitpunkt der Bestellung
customer_id / customer_unique_id – eindeutige Kundenzuordnung
seller_id – Verkäufer-ID
product_category_name_english – Produktkategorie
price, freight_value – Preis und Versandkosten
review_score – Kundenbewertung
geolocation_lat, geolocation_lng – Kunden- und Seller-Koordinaten

## 🤖 Methodik

### Data Preprocessing
Zusammenführung aller Olist-Tabellen zu einem zentralen Faktendatensatz
Entfernen unvollständiger oder fehlerhafter Zeilen

Berechnung neuer Features:
Lieferzeit (Tage)
Distanz zwischen Seller und Kunde
Umsatz pro Order
Speicherung der bereinigten Daten als Parquet unter /data/processed/

### Modeling Approach  
Explorative Datenanalyse (EDA) für Umsatz-, Liefer- und Kundentrends
Logistische Regression zur Analyse von Lieferverzögerungen
Kohortenanalyse zur Messung von Kundenbindung und Wiederkäufen
Pareto-Analysen zur Identifikation der umsatzstärksten Kategorien

### Evaluation
Statistische Auswertung von Lieferzeiten, SLA-Verletzungen und Kundenzahlen
KPI-basierte Bewertung (z. B. Retention-Rate, Umsatzverteilung, Anteil verspäteter Lieferungen)

## 📈 Ergebnisse

**Model Performance:**
<!-- Deine besten Metriken (Accuracy, RMSE, etc.) -->

**Wichtigste Visualisierungen:**
<!-- Verweis auf Key-Plots in deinen Notebooks -->

## 🚀 Reproduzierbarkeit

### Setup
```bash
# Repository klonen
git clone [DEIN-REPO-LINK]
cd [REPO-NAME]

# Dependencies installieren
uv sync
```

### Ausführung
```bash
# Notebooks in dieser Reihenfolge ausführen:
# 1. notebooks/01_exploration.ipynb
# 2. notebooks/02_preprocessing.ipynb  
# 3. notebooks/03_modeling.ipynb
# 4. notebooks/04_results.ipynb
```


## 🎓 Über dieses Projekt

**Kontext:** 
<!-- Im Rahmen welches Kurses/welcher Veranstaltung? -->

**Zeitraum:** 
<!-- Wann hast du das Projekt durchgeführt? -->

**Autor:** 
<!-- Dein Name -->

## 📞 Kontakt

**GitHub:** [@DeinUsername](https://github.com/DeinUsername)  
**E-Mail:** deine.email@beispiel.de  
**LinkedIn:** [Dein Profil](https://linkedin.com/in/dein-profil)

## 🙏 Danksagungen

<!-- Hier kannst du Personen oder Ressourcen erwähnen, die dir geholfen haben -->

---

**⭐ Wenn dir dieses Projekt gefällt, gib gerne einen Star!**
