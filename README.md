
<img src="https://github.com/openZH/covid_19/blob/master/gd.png" alt="GD-logo" width="200"/>

# Sars-Cov-2 Vaccination Registration


__DE__ : Dieses Repository enthält einen Datensatz...

__EN__ : This repository contains a dataset of adresses and coordinates of locations in the Canton of Zurich where Sars-Cov-2 vaccinations are given. 


### 1. Datensatz mit Gesamtzahlen 

| Spaltenname / Fieldname      | Beschreibung (DE)                               | Description (EN)   | Format |
|---------------------|--------------------------------------------|------------|------|
| __date__  | Datum |  |YYYY-MM-DD|
| __ncumul_secondvacc__  | Anzahl Personen die bis zum Stichtag die zweite Impfung erhalten haben |  |Zahl|
| __ncumul_firstvacc__  | Anzahl Personen die bis zum Stichtag die erste Impfung erhalten haben |  |Zahl|
| __ncumul_registered__  | Anzahl Personen die bis zum Stichtag registriert haben|  |Zahl|


### 2. Datensatz nach Altersklassen und Impfgruppen

| Spaltenname / Fieldname      | Beschreibung (DE)                               | Description (EN)   | Format |
|---------------------|--------------------------------------------|------------|------|
| __Date__  | Datum|  |YYYY-MM-DD|
| __VaccGroup__  | Gruppen gemäss Impfkampagne (ZH)  |  ||
| __AgeClass__  | Altersklassen gemäss Impfkampagne (BAG) : 18-49,50-64, 65-74, ü75|  ||
| __ncumul_secondvacc__  | Anzahl Personen die bis zum Stichtag die zweite Impfung erhalten haben |  |Zahl|
| __ncumul_firstvacc__  | Anzahl Personen die an dem Datum die erste Impfung erhalten haben |  |Zahl|
| __ncumul_registered__  | Anzahl Personen welche sich an dem Datum registriert haben aber noch nicht geimpft sind |  |Zahl|
