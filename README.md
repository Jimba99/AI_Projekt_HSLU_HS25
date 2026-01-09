# AI_Projekt_HSLU_HS25
Datenanalyse für das AI-Projekt

02.12.25 - Repository erstellt
Author: Matthias Bänziger

## Thema: 
In meinem Einzelprojekt entwickle ich ein neuronales Netz. Ziel des Modells ist es, die Anzahl Personen in einem Bild Personen vorherzusagen und diese Anzahl anschliessend in eine vordefinierte Grössenklasse einzuordnen.

Die verwendeten Grössenklassen sind wie folgt definiert:
0–10 Personen, 11–20 Personen, 21–30 Personen, 31–40 Personen, 40 Personen und mehr

Als Trainingsdatensatz werden 2000 Bilder verwendet, die zwischen 0 und maximal 55 Personen pro Bild enthalten. 
Quelle: https://www.kaggle.com/datasets/fmena14/crowd-counting/code

Zur Bewertung der Leistungsfähigkeit des selbst entwickelten Modells wird zusätzlich ein vortrainiertes Modell aus der Hugging Face Model Library eingesetzt, konkret das Modell „*yolos-small-person*“.
Quelle: https://huggingface.co/AdamCodd/yolos-small-person

Dieses Modell wird mit denselben Bilddaten evaluiert wie das selbsttrainierte neuronale Netz. Die vom YOLOS-Modell vorhergesagte Anzahl an Personen wird ebenfalls in die definierten Grössenklassen eingeteilt. Abschliessend erfolgt der Vergleich zwischen den beiden Modellen. 

## Dokumente:
YOLO-FACE_Modell.ipynb: Modell basiserend auf dem YOLO-SMALL-PERSON-MODELL. Das Modell wurde mit anderen Trainingsdaten trainiert. Die gesamte Datensatz, welcher im selbstgebauten Modell als Trainings- und Testdaten verwendet wurde. 
- **Dieses Notebook** muss zwingend in der **GPUHUB-Umgebung PYTORCH** ausgeführt werden.

AI_Einzelprojekt_selbgebautes_Modell.ipynb: Selbsterstelltes Modell basierend auf einem CNN.
- **Dieses Notebook** muss zwingend in der ** GPUHUB-Umgebung Tenserflow** ausgeführt werden.
