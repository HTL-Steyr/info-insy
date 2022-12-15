# Informationssysteme

(INSY)

---

## Stundentafel

| Gegenstand          | 1.  | 2.  | 3.  | 4.  | 5.  |
|---------------------|-----|-----|-----|-----|-----|
| Informationssysteme | -   | -   | 3   | 3   | 2   |

--

## Warum gibt es das Fach?

* Warum Datenbanksysteme?

* Theorie hinter Datenbanksystemen

* Abfragen stellen mit SQL

* Datenbanken in Verbindung mit Programmierprojekten

---

## Warum Datenbanksysteme

Heutzutage ist es nötig, ernorme Mengen an Daten zu speichern und mit diesen *effizient* arbeiten zu können.
Dafür gibt es Datenbankensysteme, wo diese strukturiert gespeichert sind und abgefragt werden können.

---
## Verschiedene Arten von DBS
- Key-Value Datenbanken
- Dokumentenbasierte Datenbanken
- Relationale Datenbanken <br /><br />
...und viele mehr. Diese haben verschiedene Vor- und Nachteile. Am weitesten verbreitet sind relationale Datenbanken,
dort werden die Daten in Tabellen (Relationen) gespeichert. Im Unterricht weden Hauptsächlich diese behandelt.
---

## Standards von Datenbanksystemen

Damit die Datenbanken einwandfrei funktionieren müssen gewisse Regelungen eingehalten werden.
Diese Regelungen kommen bei jeder professionellen Datenbank zum Einsatz und sind essenziell zu verstehen, um selbst
vernünftig mit Datenbanken arbeiten zu können.

---

## Abfragen an Datenbanken stellen mit SQL

Um mit der Datenbank zu kommunizieren, gibt es die Structured Query Language, kurz SQL.
SQL-statements schreiben kann eine hohe Komplexität annehmen und hat somit einen größeren Lernbedarf.

---

## Datenbanken in Verbindung mit Programmierprojekten

In komplexen Anwendungen stehen herkömmliches Programmieren und SQL in enger Verbindung.
Daten die z.B. über die Benutzeroberfläche einer Anwendung eingegeben werden, müssen dann über SQL-Statements in eine
Datenbank eingefügt oder aktualisiert werden.

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

**E**ntity-**R**elationship-Diagramme helfen beim planen von Datenbanken. Hierbei werden die Tabellen (Entitys)
aufgezeichnet und auf Basis der Natur ihrer Zusammenhänge (Relationships) auf verschiedene Arten verbunden.

<img src="resources/Erdiagramm.png">
---

## SQL

Verständnis der **S**tructured **Q**uery **L**anguage ist essenziell für jeden ITler.
Mit dieser Sprache kann man auf die meisten gängigen Datenbanksysteme zugreifen um Daten zu lesen oder zu schreiben.
Außerdem werden dir Eigenheiten verschiedener Datenbanksysteme beigebracht.

```sql
SELECT first_name, last_name
FROM employee e
         INNER JOIN department d ON e.abt_id = a.id
WHERE lower(m.job) = 'manager';
```

---

## JDBC / PDO

JDBC und PDO sind Zusatzfunktionalitäten für die Programmiersprachen Java und PHP. Mit ihnen wird der Datenbankzugriff
für viele Datenbanksysteme vereinheitlicht. So lassen sich leicht SQL-Statements in deinen Programmen ausführen!

```php
$dbh = new PDO('pgsql:host=xserv;dbname=pagila', "reader", "reader");
$res = $dbh->query('SELECT language_id, name from language');

while ($row = $res->fetch()) {
    echo $row['language_id'] . $row['name'];
}
```

-



