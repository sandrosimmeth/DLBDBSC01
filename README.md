# Fallstudie: Datengetriebene Strategieentwicklung für WealthyGrowth

Dies ist die Fallstudie für das Modul **Statistical Computing (DLBDBSC01)** an der IU Internationalen Hochschule.

[cite_start]Die Analyse untersucht globale Entwicklungsindikatoren, um eine datengetriebene Handlungsempfehlung für die (fiktive) NGO "WealthyGrowth" abzuleiten[cite: 165]. [cite_start]Ziel ist es, den strategischen Hebel (Bildung, Frauen-Erwerbstätigkeit oder Lebenserwartung) [cite: 168, 170, 172] [cite_start]mit dem größten positiven Einfluss auf das Wirtschaftswachstum (BIP pro Kopf) zu identifizieren[cite: 167].

## Inhalt des Repositories

* `DLBDBSC01 - test.ipynb`: Das Jupyter Notebook, das den gesamten Analyseprozess von der Datenladung bis zur Visualisierung und dem Backtest enthält.
* [cite_start]`/data/`: Enthält die Rohdaten (CSVs) von der Weltbank, die für die Analyse verwendet wurden[cite: 176].

## Analytischer Ansatz

Der im Notebook dokumentierte Prozess umfasst:

1.  [cite_start]**Datenbeschaffung und -aufbereitung**: Import der Weltbank-Daten [cite: 176] [cite_start]und Transformation ins Long-Format [cite: 683-693].
2.  [cite_start]**Datenbereinigung**: Filterung von Nicht-Länder-Aggregaten [cite: 719-729] [cite_start]und Interpolation fehlender Werte mittels linearer Regression [cite: 785-804, 180].
3.  [cite_start]**Analyse**: Eine umfassende Korrelationsanalyse (Pearson) zur Untersuchung der direkten Effekte und Interdependenzen [cite: 183, 958-974].
4.  [cite_start]**Plausibilisierung (Backtest)**: Ein quasi-experimenteller Backtest, der den kausalen Zusammenhang zwischen der Reduktion der Kindersterblichkeit und späterem BIP-Wachstum stützt [cite: 1182-1189].

## Ergebnis

Die Analyse identifiziert die **Senkung der Kindersterblichkeit** als den zentralen strategischen Hebel. [cite_start]Dieser Faktor beeinflusst nicht nur die Lebenserwartung (Hypothese C) positiv, sondern löst auch eine Kaskade aus, die die Fertilitätsrate senkt (Hypothese B) und die Einschulungsrate erhöht (Hypothese A) [cite: 1013-1017].

## Ausführung

1.  Klonen Sie das Repository.
2.  [cite_start]Stellen Sie sicher, dass die erforderlichen Python-Bibliotheken installiert sind (siehe Notebook-Imports [cite: 663-669]): `pandas`, `numpy`, `seaborn`, `scikit-learn`, `matplotlib`.
3.  Öffnen und führen Sie das Jupyter Notebook `DLBDBSC01 - test.ipynb` aus. Alle Pfade zur `/data/`-Quelle sind relativ und sollten direkt funktionieren.
