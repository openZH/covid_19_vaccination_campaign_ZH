
<img src="https://github.com/openZH/covid_19/blob/master/gd.png" alt="GD-logo" width="200"/>
<img src="https://github.com/openZH/covid_19/blob/master/statistisches_amt_kt_zh.png" alt="OpenZH-logo" width="180"/>

[![GitHub commit](https://img.shields.io/github/last-commit/openZH/covid_19)](https://github.com/openZH/covid_19_vaccination_campaign_ZH/commits/master)

__Please note:__ <br>
- Data resources in this repository by the __Division for Data Analysis of the Office of Health Care of the Canton of Zurich__ are paused (since 2022-10-12). Useful, updated data is available from the __Federal Office of Public Health (FOPH)__ as referenced [in the section 'Scope' below](https://github.com/openZH/covid_19_vaccination_campaign_ZH/tree/master#scope).
- Data structure, variables and acccess URLs of all four data resources changed to version v2 from 2021-01-12 onwards. All changes in detail: https://github.com/openZH/covid_19_vaccination_campaign_ZH/discussions/8 <br>

# Sars-Cov-2 vaccination campaign data reported by the Canton of Zurich

### Scope
This repository contains official open government data resources of the Sars-Cov-2 vaccination campaign __in the Canton of Zurich__ conducted by the __Department of Health of the Canton of Zurich__.

The data resources in this repository are a supplement to the official Sars-Cov-2 Vaccination Campaign indicators and data, which Swiss Cantons and the Principality of Liechtenstein are providing via the Federal Office of Public Health (FOPH): <br>
- [FOPH's covid19.admin.ch dashboard](https://www.covid19.admin.ch/en/epidemiologic/vacc-doses?detGeo=ZH#showDetail), vaccine doses (filtered by ZH) <br>
- [FOPH's covid19.admin.ch API documentation](https://www.covid19.admin.ch/api/data/documentation) <br>
- [FOPH's covid19.admin.ch API endpoint](https://www.covid19.admin.ch/api/data/context) <br>

__Please note:__ <br>
- Data provided in this repository and via the FOPH may differ due to different collection and publication dates as well as retroactive corrections. <br>
- Data from the first weeks of the vaccination campaign were integrated using bulk imports and then cleaned. __Retroactive corrections to the data may occur. These are made transparent with each update__ (see [last commit](https://github.com/openZH/covid_19_vaccination_campaign_ZH/commits/master)). <br>
- Values that cannot (yet) be assigned or are obviously incorrectly entered are set to 'NA'. <br>

### Update
Data resources in this repository by the __Division for Data Analysis of the Office of Health Care of the Canton of Zurich__ are paused (since 2022-10-12). Useful, updated data is available from the Federal Office of Public Health (FOPH) as referenced [in the section 'Scope' above](https://github.com/openZH/covid_19_vaccination_campaign_ZH/tree/master#scope).

### Contact

If you have questions or want to report something regarding this repository, please contact the __Specialist Unit for Open Government Data of the Canton of Zurich__ by: <br>
- [creating a GitHub issue](https://github.com/openZH/covid_19_vaccination_campaign_ZH/issues) or <br>
- write an e-mail to [info@open.zh.ch](mailto:info@open.zh.ch). <br>

Many thanks for your feedback!

<br>

## 1. Cumulative number of vaccinations of persons residing in the canton of Zurich by 1-year age groups for the most recent calendar week/ Kumulierte Anzahl Impfungen im Kanton Zürich wohnhafter Personen nach 1-Jahres-Altersklassen für die aktuellste Kalenderwoche

**Data** <br>

>**https://raw.githubusercontent.com/openZH/covid_19_vaccination_campaign_ZH/master/COVID19_Impfungen_pro_Woche_Alter_in_KTZH_wohnhaft.csv** <br>
>*Description:* cumulative numbers (1st vaccination, 2nd vaccination) up to and including the reporting date, age group <br>
>*Update frequency:* weekly <br>
>*Spatial unit:* Canton of Zurich <br>
>*Format:* csv <br>

**Metadata**

| Fieldname / Spaltenname | Description (EN)             | Beschreibung (DE)             | Format     |
|-------------------------|------------------------------|-------------------------------|------------|
| __week_from__           | Start date of week | Erster Tag der Woche | YYYY-MM-DD |
| __week_until__          | End date of week | Letzter Tag der Woche | YYYY-MM-DD |
| __calendar_week__       | Calendar week | Kalenderwoche | Number     |
| __age__                 | 1-year age classes ('0', '1', '2', .., '100+') | 1-Jahres-Altersklassen ('0', '1', '2', .., '100+') | Number |
| __ncumul_firstvacc__    | Number of persons who received the first vaccination up to and including the reporting date | Anzahl Personen, die bis und mit Stichtag die erste Impfung erhalten haben | Number     |
| __ncumul_secondvacc__   | Number of persons who received the second vaccination up to and including the reporting date | Anzahl Personen, die bis und mit Stichtag die zweite Impfung erhalten haben | Number     |

<br>

## 2. Cumulative number of vaccinations by residence per calendar week from 2021-01-18 / Kumulierte Anzahl Impfungen nach Wohnsitz pro Kalenderwoche ab 2021-01-18 

**Data** <br>

>**https://raw.githubusercontent.com/openZH/covid_19_vaccination_campaign_ZH/master/COVID19_Impfungen_pro_Woche_Wohnsitz.csv** <br>
>*Description:* detailed numbers (1st vaccination, 2nd vaccination) per calendar week, residence <br>
>*Update frequency:* weekly <br>
>*Spatial unit:* Canton of Zurich <br>
>*Format:* csv <br>

**Metadata**

| Fieldname / Spaltenname | Description (EN)             | Beschreibung (DE)             | Format     |
|-------------------------|------------------------------|-------------------------------|------------|
| __week_from__           | Start date of week | Erster Tag der Woche | YYYY-MM-DD |
| __week_until__          | End date of week | Letzter Tag der Woche | YYYY-MM-DD |
| __calendar_week__       | Calendar week | Kalenderwoche | Number     |
| __bfsNumber__           | [FSO Number](https://www.bfs.admin.ch/bfs/en/home/basics/swiss-official-commune-register.assetdetail.16924990.html), if residence is a district of Canton ZH | [BFS-Nummer](https://www.bfs.admin.ch/bfs/de/home/grundlagen/agvch.assetdetail.16924990.html), wenn Wohnort ein Bezirk des Kantons ZH ist | Number       |
| __residence__           | Residence (districts of Canton of Zurich, 'ZH aber ausserkantonal geimpft' (no residence information by district is available for Canton ZH residents vaccinated outside the canton), 'Nachbarkantone'=neighbouring cantons, 'andere Kantone'=other cantons, 'unbekannt'=unknown) | Wohnsitz (Bezirke des Kantons Zürich, 'ZH aber ausserkantonal geimpft' (von Menschen mit Wohnsitz im Kanton ZH, die ausserkantonal geimpft wurden, sind keine Wohnsitzinformationen nach Bezirken vorhanden), 'Nachbarkantone', 'andere Kantone', 'unbekannt') | Text       |
| __ncumul_firstvacc__    | Number of persons who received the first vaccination up to and including the reporting date | Anzahl Personen, die bis und mit Stichtag die erste Impfung erhalten haben | Number     |
| __ncumul_secondvacc__   | Number of persons who received the second vaccination up to and including the reporting date | Anzahl Personen, die bis und mit Stichtag die zweite Impfung erhalten haben | Number     |

<br>

## 3. Cumulative number of vaccinations by postal code per calendar week from 2021-01-18 / Kumulierte Anzahl Impfungen nach Postleitzahl pro Kalenderwoche ab 2021-01-18 

**Data** <br>

>**https://raw.githubusercontent.com/openZH/covid_19_vaccination_campaign_ZH/master/COVID19_Impfungen_pro_Woche_PLZ.csv** <br>
>*Description:* detailed numbers (1st vaccination, 2nd vaccination) per calendar week, postal code <br>
>*Update frequency:* weekly <br>
>*Spatial unit:* Canton of Zurich <br>
>*Format:* csv <br>

**Metadata**

| Fieldname / Spaltenname | Description (EN)             | Beschreibung (DE)             | Format     |
|-------------------------|------------------------------|-------------------------------|------------|
| __calendar_week__       | Calendar week | Kalenderwoche | Number     |
| __week_from__           | Start date of week | Erster Tag der Woche | YYYY-MM-DD |
| __week_until__          | End date of week | Letzter Tag der Woche | YYYY-MM-DD |
| __plz__                 | Postal code                  | Postleitzahl                  | Number     |
| __population__          | Total number of residents in the canton of Zurich in the corresponding postal code | Gesamtanzahl im Kanton Zürich wohnhafter Menschen in der entsprechenden Postleitzahl | Number     |
| __ncumul_firstvacc__    | Number of persons who received the first vaccination up to and including the reporting date | Anzahl Personen, die bis und mit Stichtag die erste Impfung erhalten haben | Number     |
| __ncumul_secondvacc__   | Number of persons who received the second vaccination up to and including the reporting date | Anzahl Personen, die bis und mit Stichtag die zweite Impfung erhalten haben | Number     |

<br>

## 4. Cumulative number of vaccinations by 10-year age groups, gender per day from 2021-01-18 / Kumulierte Anzahl Impfungen nach 10-Jahres-Altersklassen, Geschlecht pro Tag ab 2021-01-18

**Data** <br>

>**https://raw.githubusercontent.com/openZH/covid_19_vaccination_campaign_ZH/master/COVID19_Impfungen_pro_Datum_Altersklasse_Geschlecht.csv** <br>
>*Description:* detailed numbers (1st vaccination, 2nd vaccination) per day, 10-year age groups, gender <br>
>*Update frequency:* weekly <br>
>*Spatial unit:* Canton of Zurich <br>
>*Format:* csv <br>

**Metadata**

| Fieldname / Spaltenname | Description (EN)             | Beschreibung (DE)             | Format     |
|-------------------------|------------------------------|-------------------------------|------------|
| __date__                | Date | Datum | YYYY-MM-DD     |
| __ageclass__            | 10-year age classes ('0-9', '10-19', '20-29', .., '80+') | 10-Jahres-Altersklassen ('0-9', '10-19', '20-29', .., '80+') | Number (range) |
| __gender__              | Gender ('d'=diverse, 'f'=female, 'm'=male, 'NA'=unknown) | Gender ('d'=divers, 'f'=weiblich, 'm'=männlich, 'NA'=unbekannt) | Text     |
| __ncumul_firstvacc__    | Number of persons who received the first vaccination up to and including the reporting date | Anzahl Personen, die bis und mit Stichtag die erste Impfung erhalten haben | Number     |
| __ncumul_secondvacc__   | Number of persons who received the second vaccination up to and including the reporting date | Anzahl Personen, die bis und mit Stichtag die zweite Impfung erhalten haben | Number     |
