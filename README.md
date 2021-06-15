
<img src="https://github.com/openZH/covid_19/blob/master/gd.png" alt="GD-logo" width="200"/>
<img src="https://github.com/openZH/covid_19/blob/master/statistisches_amt_kt_zh.png" alt="OpenZH-logo" width="180"/>

[![GitHub commit](https://img.shields.io/github/last-commit/openZH/covid_19)](https://github.com/openZH/covid_19_vaccination_campaign_ZH/commits/master)

# Sars-Cov-2 vaccination campaign data reported by the Canton of Zurich

### Scope
This repository contains official open government data resources of the Sars-Cov-2 vaccination campaign __in the Canton of Zurich__ conducted by the __Department of Health of the Canton of Zurich__.

The data resources in this repository are a supplement to the official Sars-Cov-2 Vaccination Campaign indicators and data, which Swiss Cantons and the Principality of Liechtenstein are providing via the Federal Office of Public Health (FOPH): <br>
- [FOPH's covid19.admin.ch dashboard](https://www.covid19.admin.ch/en/epidemiologic/vacc-doses?detGeo=ZH#showDetail), vaccine doses (filtered by ZH) <br>
- [FOPH's covid19.admin.ch API documentation](https://www.covid19.admin.ch/api/data/documentation) <br>
- [FOPH's covid19.admin.ch API endpoint](https://www.covid19.admin.ch/api/data/context) <br>

__Please note:__ <br>
- Data provided in this repository and via the FOPH may differ due to different collection and publication dates as well as retroactive corrections. <br>
- Data from the first weeks of the vaccination campaign were integrated using bulk imports and then cleaned. This process is still ongoing. __Retroactive corrections to the data may occur. These are made transparent with each update__ (see [last commit](https://github.com/openZH/covid_19_vaccination_campaign_ZH/commits/master)). <br>
- Values that cannot (yet) be assigned or are obviously incorrectly entered are set to 'NA'. <br>

### Update
Data resources in this repository are updated on weekdays by the __Division for Data Analysis of the Office of Health Care of the Canton of Zurich__ according to the specifications below; i.e. (a) once a day respectively (b) once per week.

### Contact

If you have questions or want to report something regarding this repository, please contact the __Specialist Unit for Open Government Data of the Canton of Zurich__ by: <br>
- [creating a GitHub issue](https://github.com/openZH/covid_19_vaccination_campaign_ZH/issues) or <br>
- write an e-mail to [info@open.zh.ch](mailto:info@open.zh.ch). <br>

Many thanks for your feedback!

<br>

## 1. Cumulative number of vaccinations by vaccination groups / Kumulierte Anzahl Impfungen nach Impfgruppen

**Data** <br>

>**https://github.com/openZH/covid_19_vaccination_campaign_ZH/tree/master/...** <br>
>*Description:* detailed numbers (1st vaccination, 2nd vaccination) up to and including the reporting date, vaccination group <br>
>*Update frequency:* daily (on weekdays) <br>
>*Spatial unit:* Canton of Zurich <br>
>*Format:* csv <br>

**Metadata**

| Fieldname / Spaltenname | Description (EN)             | Beschreibung (DE)             | Format     |
|-------------------------|------------------------------|-------------------------------|------------|
| __date__                | Reporting date (earlier than 2021-01-04 are accumulated to 'n.a.') | Stichtag (frühere als 2021-01-04 sind unter 'n.a.' kumuliert) | YYYY-MM-DD |
| __vaccgroup_zh__        | Vaccination group ('A' to 'T') according to [categorisation of the Canton of Zurich](https://www.zh.ch/de/gesundheit/coronavirus/coronavirus-impfung/impfgruppen.html#main_table_copy_copy) | Impfgruppe ('A' bis 'T') gemäss [Kategorisierung des Kantons Zürich](https://www.zh.ch/de/gesundheit/coronavirus/coronavirus-impfung/impfgruppen.html#main_table_copy_copy) | Text |
| __ncumul_firstvacc__    | Number of persons who received the first vaccination up to and including the reporting date | Anzahl Personen, die bis und mit Stichtag die erste Impfung erhalten haben | Number     |
| __ncumul_secondvacc__   | Number of persons who received the second vaccination up to and including the reporting date | Anzahl Personen, die bis und mit Stichtag die zweite Impfung erhalten haben | Number     |

<br>

## 2. Cumulative number of vaccinations by 10-year age groups, gender / Kumulierte Anzahl Impfungen nach 10-Jahres-Altersklasse, Geschlecht

**Data** <br>

>**https://github.com/openZH/covid_19_vaccination_campaign_ZH/tree/master/...** <br>
>*Description:* detailed numbers (1st vaccination, 2nd vaccination) up to and including the reporting date, age group, gender <br>
>*Update frequency:* daily (on weekdays) <br>
>*Spatial unit:* Canton of Zurich <br>
>*Format:* csv <br>

**Metadata**

| Fieldname / Spaltenname | Description (EN)             | Beschreibung (DE)             | Format     |
|-------------------------|------------------------------|-------------------------------|------------|
| __date__                | Reporting date (earlier than 2021-01-04 are accumulated to 'n.a.') | Stichtag (frühere als 2021-01-04 sind unter 'n.a.' kumuliert) | YYYY-MM-DD |
| __ageclass__            | 10-year age classes ('0-9', '10-19', '20-29', .., '80+') | 10-Jahres-Altersklassen ('0-9', '10-19', '20-29', .., '80+') | Text |
| __gender__              | Gender ('d'=diverse, 'f'=female, 'm'=male) | Geschlecht ('d'=divers, 'f'=weiblich, 'm'=männlich) | Text       |
| __ncumul_firstvacc__    | Number of persons who received the first vaccination up to and including the reporting date | Anzahl Personen, die bis und mit Stichtag die erste Impfung erhalten haben | Number     |
| __ncumul_secondvacc__   | Number of persons who received the second vaccination up to and including the reporting date | Anzahl Personen, die bis und mit Stichtag die zweite Impfung erhalten haben | Number     |

<br>

## 3. Cumulative number of vaccinations by residence per calendar week / Kumulierte Anzahl Impfungen nach Wohnsitz pro Kalenderwoche

**Data** <br>

>**https://github.com/openZH/covid_19_vaccination_campaign_ZH/tree/master/...** <br>
>*Description:* detailed numbers (1st vaccination, 2nd vaccination) per calendar week, residence <br>
>*Update frequency:* weekly (weekday *to be defined*) <br>
>*Spatial unit:* Canton of Zurich <br>
>*Format:* csv <br>

**Metadata**

| Fieldname / Spaltenname | Description (EN)             | Beschreibung (DE)             | Format     |
|-------------------------|------------------------------|-------------------------------|------------|
| __week_from__           | Start date of week (earlier than 2021-01-04 are accumulated to 'n.a.') | Erster Tag der Woche (frühere als 2021-01-04 sind unter 'n.a.' kumuliert) | YYYY-MM-DD |
| __week_until__          | End date of week (earlier than 2021-01-04 are accumulated to 'n.a.')   | Letzter Tag der Woche (frühere als 2021-01-04 sind unter 'n.a.' kumuliert) | YYYY-MM-DD |
| __calendar_week__       | Calendar week (earlier than 2021-01-04 are accumulated to 'n.a.')      | Kalenderwoche (frühere als 2021-01-04 sind unter 'n.a.' kumuliert) | Number     |
| __bfsNumber__           | [FSO Number](https://www.bfs.admin.ch/bfs/en/home/basics/swiss-official-commune-register.assetdetail.16924990.html), if residence is a district of Canton ZH |	[BFS-Nummer](https://www.bfs.admin.ch/bfs/de/home/grundlagen/agvch.assetdetail.16924990.html), wenn Wohnort ein Bezirk des Kantons ZH ist | Number       |
| __residence__           | Residence (districts of Canton of Zurich, 'Nachbarkantone'=neighbouring cantons, 'andere Kantone'=other cantons, 'unbekannt'=unknown) | Wohnsitz (Bezirke des Kantons Zürich, 'Nachbarkantone', 'andere Kantone', 'unbekannt') | Text       |
| __ncumul_firstvacc__    | Number of persons who received the first vaccination up to and including the reporting date | Anzahl Personen, die bis und mit Stichtag die erste Impfung erhalten haben | Number     |
| __ncumul_secondvacc__   | Number of persons who received the second vaccination up to and including the reporting date | Anzahl Personen, die bis und mit Stichtag die zweite Impfung erhalten haben | Number     |

<br>

## 4. Cumulative number of registrations (and vaccinations) by vaccination groups / Kumulierte Anzahl Registrierungen (und Impfungen) nach Impfgruppen

**Data** <br>

>**https://github.com/openZH/covid_19_vaccination_campaign_ZH/tree/master/...** <br>
>*Description:* detailed numbers (registrations, 1st vaccination, 2nd vaccination) up to and including the reporting date, vaccination group <br>
>*Update frequency:* daily (on weekdays) <br>
>*Spatial unit:* Canton of Zurich <br>
>*Format:* csv <br>

**Metadata**

| Fieldname / Spaltenname | Description (EN)             | Beschreibung (DE)             | Format     |
|-------------------------|------------------------------|-------------------------------|------------|
| __date__                | Reporting date (earlier than 2021-01-04 are accumulated to 'n.a.') | Stichtag (frühere als 2021-01-04 sind unter 'n.a.' kumuliert) | YYYY-MM-DD |
| __vaccgroup_zh__        | Vaccination group ('A' to 'T') according to [categorisation of the Canton of Zurich](https://www.zh.ch/de/gesundheit/coronavirus/coronavirus-impfung/impfgruppen.html) | Impfgruppe ('A' bis 'T') gemäss [Kategorisierung des Kantons Zürich](https://www.zh.ch/de/gesundheit/coronavirus/coronavirus-impfung/impfgruppen.html) | Text |
| __ncumul_registered__   | Number of persons who registered for vaccination up to and including the reporting date | Anzahl Personen, die sich bis und mit Stichtag für die Impfung registriert haben | Number |
| __ncumul_firstvacc__    | Number of persons who received the first vaccination up to and including the reporting date | Anzahl Personen, die bis und mit Stichtag die erste Impfung erhalten haben | Number     |
| __ncumul_secondvacc__   | Number of persons who received the second vaccination up to and including the reporting date | Anzahl Personen, die bis und mit Stichtag die zweite Impfung erhalten haben | Number     |

<br>

## 5. Cumulative number of registrations (and vaccinations) by 10-year age groups, gender / Kumulierte Anzahl Registrierungen (und Impfungen) nach 10-Jahres-Altersklasse, Geschlecht

**Data** <br>

>**https://github.com/openZH/covid_19_vaccination_campaign_ZH/tree/master/...** <br>
>*Description:* detailed numbers (registrations, 1st vaccination, 2nd vaccination) up to and including the reporting date, age group, gender <br>
>*Update frequency:* daily (on weekdays) <br>
>*Spatial unit:* Canton of Zurich <br>
>*Format:* csv <br>

**Metadata**

| Fieldname / Spaltenname | Description (EN)             | Beschreibung (DE)             | Format     |
|-------------------------|------------------------------|-------------------------------|------------|
| __date__                | Reporting date (earlier than 2021-01-04 are accumulated to 'n.a.') | Stichtag (frühere als 2021-01-04 sind unter 'n.a.' kumuliert) | YYYY-MM-DD |
| __ageclass__            | 10-year age classes ('0-9', '10-19', '20-29', .., '80+') | 10-Jahres-Altersklassen ('0-9', '10-19', '20-29', .., '80+') | Text |
| __gender__              | Gender (..)                  | Geschlecht (..)               | Text       |
| __ncumul_registered__   | Number of persons who registered for vaccination up to and including the reporting date | Anzahl Personen, die sich bis und mit Stichtag für die Impfung registriert haben | Number |
| __ncumul_firstvacc__    | Number of persons who received the first vaccination up to and including the reporting date | Anzahl Personen, die bis und mit Stichtag die erste Impfung erhalten haben | Number     |
| __ncumul_secondvacc__   | Number of persons who received the second vaccination up to and including the reporting date | Anzahl Personen, die bis und mit Stichtag die zweite Impfung erhalten haben | Number     |
