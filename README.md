
<img src="https://github.com/openZH/covid_19/blob/master/gd.png" alt="GD-logo" width="200"/>
<img src="https://github.com/openZH/covid_19/blob/master/statistisches_amt_kt_zh.png" alt="OpenZH-logo" width="180"/>

[![GitHub commit](https://img.shields.io/github/last-commit/openZH/covid_19)](https://github.com/openZH/covid_19_vaccination_campaign_ZH/commits/master)

# Sars-Cov-2 Vaccination Campaign open government data reported by the Canton of Zurich

### Scope
This repository contains official open government data resources of the Sars-Cov-2 vaccination campaign __in the Canton of Zurich__ conducted by the Department of Health of the Canton of Zurich.

The data resources in this repository are a supplement to the official Sars-Cov-2 Vaccination Campaign indicators and data, which Swiss Cantons and the Principality of Liechtenstein are providing via the Federal Office of Public Health (FOPH): <br>
- [FOPH's covid19.admin.ch dashboard](https://www.covid19.admin.ch/en/epidemiologic/vacc-doses?detGeo=ZH#showDetail), vaccine doses (filtered by ZH) <br>
- [FOPH's covid19.admin.ch API](https://www.covid19.admin.ch/api/data/context) <br>

__Please note:__ Data provided in this repository and via the FOPH may differ due to different collection and publication dates as well as retroactive corrections. <br>

### Update
Data resources in this repository are updated on weekdays by the Division for Data Analysis of the Office of Health Care of the Canton of Zurich according to the specification in their description (a) once a day respectively (b) once per week.

All (i.e. retroactive) data corrections are made transparent with each update (see [last commit](https://github.com/openZH/covid_19_vaccination_campaign_ZH/commits/master)).

### Contact

If you have questions regarding this repository, please contact the Specialist Unit for Open Government Data of the Canton of Zurich: <br>
- [twitter.com/OpenDataZH](https://twitter.com/OpenDataZH) <br>
- [info@open.zh.ch](mailto:info@open.zh.ch) <br>


## 1. Canton of Zurich: Vaccinations per date and vaccination group / Impfungen pro Datum und Impfgruppe

**Data** <br>

>**https://github.com/openZH/covid_19_vaccination_campaign_ZH/tree/master/COVID19_vaccination_ZH_vaccgroup_example.csv** <br>
>*Description:* __Example file__ of detailed numbers (1st vaccination, 2nd vaccination) up to and including the reporting date, vaccination group <br>
>*Update frequency:* daily (on weekdays) <br>
>*Spatial unit:* Canton of Zurich <br>
>*Format:* csv <br>

**Metadata**

| Fieldname / Spaltenname | Description (EN)             | Beschreibung (DE)             | Format     |
|-------------------------|------------------------------|-------------------------------|------------|
| __date__                | Reporting date               | Stichtag                      | YYYY-MM-DD |
| __vaccgroup_zh__        | Vaccination group ('A' to 'T') according to [categorisation of the Canton of Zurich](https://www.zh.ch/de/gesundheit/coronavirus/coronavirus-impfung.html#-72400422) | Impfgruppe ('A' bis 'T') gemäss [Kategorisierung des Kantons Zürich](https://www.zh.ch/de/gesundheit/coronavirus/coronavirus-impfung.html#-72400422) | Text |
| __ncumul_firstvacc__    | Number of persons who received the first vaccination up to and including the reporting date | Anzahl Personen, die bis und mit Stichtag die erste Impfung erhalten haben | Number     |
| __ncumul_secondvacc__   | Number of persons who received the second vaccination up to and including the reporting date | Anzahl Personen, die bis und mit Stichtag die zweite Impfung erhalten haben | Number     |


## 2. Canton of Zurich: Detailed resource vaccinations / Detailierte Ressource Impfungen

**Data** <br>

>**https://github.com/openZH/covid_19_vaccination_campaign_ZH/tree/master/COVID19_vaccination_ZH_detailed_example.csv** <br>
>*Description:* __Example file__ of detailed numbers per day (1st vaccination, 2nd vaccination), vaccination group, age class, gender, canton of residence, place (type) of vaccination, vaccine code (Global Trade Item Number, GTIN) <br>
>*Update frequency:* weekly (weekday *yet to be defined*) <br>
>*Spatial unit:* Canton of Zurich <br>
>*Format:* csv <br>

**Metadata**

| Fieldname / Spaltenname | Description (EN)             | Beschreibung (DE)             | Format     |
|-------------------------|------------------------------|-------------------------------|------------|
| __date__                | Reporting date               | Stichtag                      | YYYY-MM-DD |
| __vaccgroup_zh__        | Vaccination group ('A' to 'T') according to [categorisation of the Canton of Zurich](https://www.zh.ch/de/gesundheit/coronavirus/coronavirus-impfung.html#-72400422) | Impfgruppe ('A' bis 'T') gemäss [Kategorisierung des Kantons Zürich](https://www.zh.ch/de/gesundheit/coronavirus/coronavirus-impfung.html#-72400422) | Text |
| __ageclass__            | 10-year age classes ('0-9', '10-19', '20-29', .., '80+') | 10-Jahres-Altersklassen ('0-9', '10-19', '20-29', .., '80+') | Text |
| __gender__              | Gender (..)                  | Geschlecht (..)               | Text       |
| __residence__           | Canton of residence (abbreviation of canton, 'andere' for foreigners without residence, or 'unbekannt') | Wohnkanton (Kantonskürzel, 'andere' für Personen ohne Wohnsitz in der Schweiz) oder 'unbekannt' | Text       |
| __vaccplace_zh__        | Place (type) of vaccination ('Impfzentrum', 'Alters_und_Pflegeheim, 'Arztpraxis', 'Apotheke', 'Spital' or 'andere') | Ort (Typ) der Impfung ('Impfzentrum', 'Alters_und_Pflegeheim, 'Arztpraxis', 'Apotheke', 'Spital' oder 'anderer') | Text       |
| __vacccode__            | Vaccine code (Global Trade Item Number, GTIN) | Impfstoff Code (Global Trade Item Number, GTIN) | Text       |
| __ncumul_firstvacc__    | Number of persons who received the first vaccination up to and including the reporting date | Anzahl Personen, die bis und mit Stichtag die erste Impfung erhalten haben | Number     |
| __ncumul_secondvacc__   | Number of persons who received the second vaccination up to and including the reporting date | Anzahl Personen, die bis und mit Stichtag die zweite Impfung erhalten haben | Number     |
|                         |                              |                               |            |




| __ncumul_registered__   | Number of people who registered for vaccination up to and including the reporting date | Anzahl Personen, die sich bis und mit Stichtag für die Impfung registriert haben | Number |
