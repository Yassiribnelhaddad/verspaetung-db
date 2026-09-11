# Analyse der Verspätungen der Deutschen Bahn

Ein kleines Projekt zur Daten- und Prozessanalyse: Wie pünktlich sind die Züge der Deutschen Bahn, und wo entstehen die Verspätungen?

## Fragestellungen

1. Wie hoch ist die Pünktlichkeitsquote (Verspätung unter 6 Minuten)?
2. Welche Zugtypen (ICE, IC, RE, S ...) sind am unpünktlichsten?
3. An welchen Bahnhöfen gibt es die meisten Verspätungen?
4. Zu welcher Tageszeit und an welchem Wochentag sind die Verspätungen am größten?
5. Wächst die Verspätung entlang der Fahrt eines Zuges an?

## Daten

- Quelle: [piebro/deutsche-bahn-data](https://huggingface.co/datasets/piebro/deutsche-bahn-data) (Timetables API der Deutschen Bahn)
- Lizenz: CC BY 4.0, Deutsche Bahn
- Zeitraum: Oktober 2025, ca. 100 größte Bahnhöfe
- Die Rohdaten liegen nicht im Repository. Download:

```powershell
curl.exe -L -o data/data-2025-10.parquet "https://huggingface.co/datasets/piebro/deutsche-bahn-data/resolve/main/monthly_processed_data/data-2025-10.parquet"
```

## Struktur

```
data/        Rohdaten (nicht im Repository)
notebooks/   Jupyter-Notebooks mit der Analyse
grafiken/    Exportierte Diagramme
```

## Werkzeuge

Python, pandas, matplotlib, seaborn, Jupyter
