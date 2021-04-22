
<img src="https://github.com/openZH/covid_19/blob/master/gd.png" alt="GD-logo" width="200"/>
<img src="https://github.com/openZH/covid_19/blob/master/statistisches_amt_kt_zh.png" alt="OpenZH-logo" width="180"/>

[![GitHub commit](https://img.shields.io/github/last-commit/openZH/covid_19)](https://github.com/openZH/covid_19_vaccination_campaign_ZH/commits/master)

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

__Please note:__ Data provided in this repository and via the FOPH may differ due to different collection and publication dates as well as retroactive corrections. <br>


## Canton of Zurich: Summarised ressource / Zusammengefasste Ressource

**Data** <br>

>**https://github.com/openZH/covid_19_vaccination_campaign_ZH/tree/master/COVID19_vaccination_ZH_summarised_example.csv** <br>
>*Description:* __Example file__ of summarised numbers per day <br>
>*Spatial unit:* Canton of Zurich <br>
>*Format:* csv <br>

**Metadata**

| Fieldname / Spaltenname | Description (EN)             | Beschreibung (DE)             | Format     |
|-------------------------|------------------------------|-------------------------------|------------|
| __date__                | Reporting date               | Stichtag                      | YYYY-MM-DD |
| __ncumul_registered__   | Number of people who registered for vaccination up to and including the reporting date | Anzahl Personen, die sich bis und mit Stichtag für die Impfung registriert haben | Number |
| __ncumul_firstvacc__    | Number of persons who received the first vaccination up to and including the reporting date | Anzahl Personen, die bis und mit Stichtag die erste Impfung erhalten haben | Number |
| __ncumul_secondvacc__   | Number of persons who received the second vaccination up to and including the reporting date | Anzahl Personen, die bis und mit Stichtag die zweite Impfung erhalten haben | Number |
|                         |                              |                               |            |


## 2. Datensatz nach Altersklassen und Impfgruppen

| Spaltenname / Fieldname      | Beschreibung (DE)                               | Description (EN)   | Format |
|---------------------|--------------------------------------------|------------|------|
| __date__  | Stichtag|  |YYYY-MM-DD|
| __vaccgroup_ZH__  | Gruppen gemäss Impfkampagne (ZH)  |  ||
| __agecat__  | Altersklassen gemäss Impfkampagne (BAG) : 18-49,50-64, 65-74, ü75|  ||
| __ncumul_secondvacc__  | Anzahl Personen die bis zum Stichtag die zweite Impfung erhalten haben |  |Zahl|
| __ncumul_firstvacc__  | Anzahl Personen die an dem Datum die erste Impfung erhalten haben |  |Zahl|
| __ncumul_registered__  | Anzahl Personen welche sich an dem Datum registriert haben aber noch nicht geimpft sind |  |Zahl|
