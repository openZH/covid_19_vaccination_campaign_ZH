
<img src="https://github.com/openZH/covid_19/blob/master/gd.png" alt="GD-logo" width="200"/>

# Sars-Cov-2 Vaccination Campaign open government data reported by the Canton of Zurich

This repository contains open government data ressources of the Sars-Cov-2 vaccination campaign in the Canton of Zurich conducted by the Department of Health of the Canton of Zurich. It is a supplement to the data provided via the Federal Office of Public Health (FOPH): <br>
- [FOPH's covid19.admin.ch dashboard, vaccine doses (filtered by ZH)](https://www.covid19.admin.ch/en/epidemiologic/vacc-doses?detGeo=ZH#showDetail) <br>
- [FOPH's covid19.admin.ch API](https://www.covid19.admin.ch/api/data/context) <br>

The data provided in this repository and via the FOPH may differ due to different collection and publication dates as well as retroactive corrections.

Data ressources in this repository are updated daily (on weekdays) by the Division for Data Analysis of the Office of Health Care of the Canton of Zurich. If you have questions regarding this repository, please contact the Specialist Unit for Open Government Data of the Canton of Zurich: <br>
- [twitter.com/OpenDataZH](https://twitter.com/OpenDataZH) <br>
- [info@open.zh.ch](mailto:info@open.zh.ch) <br>


## 1. Datensatz mit Gesamtzahlen 

| Spaltenname / Fieldname      | Beschreibung (DE)                               | Description (EN)   | Format |
|---------------------|--------------------------------------------|------------|------|
| __date__  | Stichtag |  |YYYY-MM-DD|
| __time__  | Publikationszeitpunkt (Uhrzeit)  |  |HH:MM|
| __ncumul_secondvacc__  | Anzahl Personen die bis zum Stichtag die zweite Impfung erhalten haben |  |Zahl|
| __ncumul_firstvacc__  | Anzahl Personen die bis zum Stichtag die erste Impfung erhalten haben |  |Zahl|
| __ncumul_registered__  | Anzahl Personen die bis zum Stichtag registriert haben|  |Zahl|


## 2. Datensatz nach Altersklassen und Impfgruppen

| Spaltenname / Fieldname      | Beschreibung (DE)                               | Description (EN)   | Format |
|---------------------|--------------------------------------------|------------|------|
| __date__  | Stichtag|  |YYYY-MM-DD|
| __time__  | Publikationszeitpunkt (Uhrzeit) |  |HH:MM|
| __vaccgroup_ZH__  | Gruppen gemäss Impfkampagne (ZH)  |  ||
| __agecat__  | Altersklassen gemäss Impfkampagne (BAG) : 18-49,50-64, 65-74, ü75|  ||
| __ncumul_secondvacc__  | Anzahl Personen die bis zum Stichtag die zweite Impfung erhalten haben |  |Zahl|
| __ncumul_firstvacc__  | Anzahl Personen die an dem Datum die erste Impfung erhalten haben |  |Zahl|
| __ncumul_registered__  | Anzahl Personen welche sich an dem Datum registriert haben aber noch nicht geimpft sind |  |Zahl|
