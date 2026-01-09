# AI_Projekt_HSLU_HS25
Datenanalyse für das AI-Projekt

02.12.25 - Repository erstellt
Author: Matthias Bänziger

# Thema: 
In meinem Einzelprojekt entwickle ich ein neuronales Netz. Ziel des Modells ist es, die Anzahl Personen in einem Bild Personen vorherzusagen und diese Anzahl anschliessend in eine vordefinierte Grössenklasse einzuordnen.

Die verwendeten Grössenklassen sind wie folgt definiert:
0–10 Personen, 11–20 Personen, 21–30 Personen, 31–40 Personen, 40 Personen und mehr

Als Trainingsdatensatz werden 2000 Bilder verwendet, die zwischen 0 und maximal 55 Personen pro Bild enthalten. (Verlinkung zum Trainingsdatensatz).

Zur Bewertung der Leistungsfähigkeit des selbst entwickelten Modells wird zusätzlich ein vortrainiertes Modell aus der Hugging Face Model Library eingesetzt, konkret das Modell „*yolos-small-person*“. Dieses Modell wird mit denselben Bilddaten evaluiert wie das selbsttrainierte neuronale Netz. Die vom YOLOS-Modell vorhergesagte Anzahl an Personen wird ebenfalls in die definierten Grössenklassen eingeteilt.  Abschliessend erfolgt der Vergleich zwischen den beiden 
