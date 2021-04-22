
<img src="https://github.com/openZH/covid_19/blob/master/gd.png" alt="GD-logo" width="200"/>

# Sars-Cov-2 Vaccination Campaign open government data reported by the Canton of Zurich

This repository contains official open government data ressources of the Sars-Cov-2 vaccination campaign __in the Canton of Zurich__ conducted by the Department of Health of the Canton of Zurich. <br>
- Data ressources in this repository are updated once a day (on weekdays) by the Division for Data Analysis of the Office of Health Care of the Canton of Zurich. <br>
- Date and time of publication, and data corrections of ressources are made transparent with each update. <br>

If you have questions regarding this repository, please contact the Specialist Unit for Open Government Data of the Canton of Zurich: <br>
- [twitter.com/OpenDataZH](https://twitter.com/OpenDataZH) <br>
- [info@open.zh.ch](mailto:info@open.zh.ch) <br>

### Further official Sars-Cov-2 Vaccination Campaign indicators and data of Swiss Cantons

The data ressources in this repository are a supplement to the official Sars-Cov-2 vaccination campaign indicators and data, which Swiss Cantons and the Principality of Liechtenstein are providing via the Federal Office of Public Health (FOPH): <br>
- [FOPH's covid19.admin.ch dashboard](https://www.covid19.admin.ch/en/epidemiologic/vacc-doses?detGeo=ZH#showDetail), vaccine doses (filtered by ZH) <br>
- [FOPH's covid19.admin.ch API](https://www.covid19.admin.ch/api/data/context) <br>

__Please note:__ The data ressources provided in this repository and via the FOPH may differ due to different collection and publication dates as well as retroactive corrections.

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
