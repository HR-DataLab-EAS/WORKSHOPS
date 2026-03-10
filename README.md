# IMAGES-FILES-BML-PROJECTEN

Met deze repository kun je **images** en **files** (zoals `.json` en `.csv`) online beschikbaar stellen voor BML‑projecten.

## Structuur van de repository

- `IMAGES`  
  Bevat afbeeldingen (bijv. `.png`, `.jpg`) die vanuit notebooks, scripts of webapplicaties benaderd kunnen worden.

- `FILES`  
  Bevat overige bestanden zoals `.json`, `.csv` en andere data- of configuratiebestanden.

- `LICENSE`  
  Informatie over de licentie (CC0-1.0).

- `README.md`  
  Dit bestand, met uitleg over gebruik en structuur.

## Bestanden uploaden (via GitHub webinterface)

1. Navigeer in de repository naar de map `IMAGES` of `FILES`.
2. Klik op **Add file** → **Upload files**.
3. Sleep één of meer bestanden naar het uploadvenster of kies ze via de bestandskiezer.
4. Controleer of de bestanden in de juiste map staan.
5. Vul een korte, duidelijke commit message in (bijv. `Add nieuwe images voor project X`).
6. Klik op **Commit changes** om de upload op te slaan.

> Tip: je kunt submappen maken door in de bestandsnaam een pad te gebruiken, bijvoorbeeld `project1/example.png`.

## Bestanden downloaden (via GitHub webinterface)

- Enkel bestand:
  1. Klik in de repository op het gewenste bestand in `IMAGES` of `FILES`.
  2. Klik op de knop **Download** (of op **View raw** en sla het bestand op via de browser).

- Hele repository:
  1. Ga naar de hoofdpagina van de repository.
  2. Klik op de groene knop **Code**.
  3. Kies **Download ZIP** en pak het ZIP‑bestand lokaal uit.

## Bestanden downloaden in code

### Voorbeeld: CSV-bestand met Python (pandas)

```python
import pandas as pd

url = "https://raw.githubusercontent.com/HR-DataLab-EAS/IMAGES-FILES-BML-PROJECTEN/main/FILES/data.csv"
df = pd.read_csv(url)
print(df.head())
