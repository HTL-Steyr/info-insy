# Informationssysteme

(INSY)

---

## Stundentafel

| Gegenstand          | 1.  | 2.  | 3.  | 4.  | 5.  |
|---------------------|-----|-----|-----|-----|-----|
| Informationssysteme | -   | -   | 3   | 3   | 2   |

--

## Warum gibt es das Fach?

* Was sind Datenbanken?

* Warum brauchen wir Datenbanksysteme?

* Theorie hinter Datenbanksystemen

* Datenbankzugriffe mit SQL

* Datenbanken in Verbindung mit Programmierprojekten

---

## Was sind Datenbanken?

**Datenbanken** ermöglichen es große Mengen an Daten strukturiert zu speichern. 
Das darum aufgebaute **D**aten**b**ank**s**ystem ermöglich das Einfügen, Lesen,
Verändern und Löschen der Daten und kümmert sich dabei auch um z.B. Events und 
Trigger, welche automatisch ausgeführt werden. 

---

## Warum brauchen wir Datenbanksysteme?

Heutzutage ist es nötig, enorme Mengen an Daten zu speichern und diese *effizient* verarbeiten zu können.
In Datenbanksystemen können diese strukturiert gespeichert sowie abgefragt werden.

---
## Verschiedene Arten von DBS
- Key-Value Datenbanken
- Dokumentenbasierte Datenbanken
- Relationale Datenbanken <br /><br />
...und viele mehr. Diese haben verschiedene Vor- und Nachteile. Am weitesten verbreitet sind relationale Datenbanken,
dort werden die Daten in Tabellen (Relationen) gespeichert. Im Unterricht werden hauptsächlich diese behandelt.
---

## Standards von Datenbanksystemen

Damit die Datenbanken einwandfrei funktionieren müssen gewisse Regelungen eingehalten werden.
Diese Regeln kommen bei jeder Datenbank zum Einsatz und bilden das Fundament für die Datenbank.

---

## Datebankzugriffe mit SQL

Mittels SQL-Statements kann man Daten in die Datenbank lesen, schreiben, verändern und löschen.

---

## Datenbanken in Verbindung mit Programmierprojekten
Hinter den meisten Anwendungen kommen Datenbanken zum Einsatz.
Daten die z.B. über die Benutzeroberfläche einer Anwendung eingegeben werden,
werden dann über diese Datenbanken verwaltet.

--

# Technologien

Was erwartet dich?

---

## Microsoft Access

Access bietet einen angenehmen Einstieg ins praktische Arbeiten
mit Datenbanken. Durch die gewohnte Office-Oberfläche wird man
nicht ins kalte Wasser geworfen. <br />
![MS Access Logo](https://upload.wikimedia.org/wikipedia/commons/thumb/f/f1/Microsoft_Office_Access_%282019-present%29.svg/180px-Microsoft_Office_Access_%282019-present%29.svg.png) <br />
<small>[Bildquelle](https://upload.wikimedia.org/wikipedia/commons/thumb/f/f1/Microsoft_Office_Access_%282019-present%29.svg/180px-Microsoft_Office_Access_%282019-present%29.svg.png)</small>

---

## ER-Diagramme

**E**ntity-**R**elationship-Diagramme helfen beim Planen von Datenbanken. In ER-Diagrammen werden die Tabellen (Entities)
und ihre Abhängigkeiten/Zusammenhänge (Relationships) visualisiert.

<img src="resources/Erdiagramm.png">
---

## SQL

Verständnis der **S**tructured **Q**uery **L**anguage ist essenziell für den Umgang mit Datenbanken.
Mit SQL kann man auf Datenbanksysteme zugreifen und Daten lesen, schreiben, löschen und aktualisieren.

```sql
SELECT first_name, last_name
FROM employee e
         INNER JOIN department d ON e.abt_id = a.id
WHERE lower(m.job) = 'manager';
```
