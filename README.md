# Fallstudie: Datengetriebene Strategieentwicklung für WealthyGrowth

Dies ist die Fallstudie für das Modul **Statistical Computing (DLBDBSC01)** an der IU Internationalen Hochschule.

Die Analyse untersucht globale Entwicklungsindikatoren, um eine datengetriebene Handlungsempfehlung für die (fiktive) NGO "WealthyGrowth" abzuleiten. Ziel ist es, den strategischen Hebel (Bildung, Frauen-Erwerbstätigkeit oder Lebenserwartung) mit dem größten positiven Einfluss auf das Wirtschaftswachstum (BIP pro Kopf) zu identifizieren.

## Inhalt des Repositories

* `DLBDBSC01 - test.ipynb`: Das Jupyter Notebook, das den gesamten Analyseprozess von der Datenladung bis zur Visualisierung und dem Backtest enthält.
* [cite_start]`/data/`: Enthält die Rohdaten (CSVs) von der Weltbank, die für die Analyse verwendet wurden.

## Analytischer Ansatz

Der im Notebook dokumentierte Prozess umfasst:

1.  **Datenbeschaffung und -aufbereitung**: Import der Weltbank-Daten und Transformation ins Long-Format.
2.  **Datenbereinigung**: Filterung von Nicht-Länder-Aggregaten und Interpolation fehlender Werte mittels linearer Regression.
3.  **Analyse**: Eine umfassende Korrelationsanalyse (Pearson) zur Untersuchung der direkten Effekte und Interdependenzen.
4.  **Plausibilisierung (Backtest)**: Ein quasi-experimenteller Backtest, der den kausalen Zusammenhang zwischen der Reduktion der Kindersterblichkeit und späterem BIP-Wachstum stützt.

## Ergebnis

Die Analyse identifiziert die **Senkung der Kindersterblichkeit** als den zentralen strategischen Hebel. Dieser Faktor beeinflusst nicht nur die Lebenserwartung (Hypothese C) positiv, sondern löst auch eine Kaskade aus, die die Fertilitätsrate senkt (Hypothese B) und die Einschulungsrate erhöht (Hypothese A).
