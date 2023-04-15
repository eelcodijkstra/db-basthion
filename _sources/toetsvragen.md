# Opdrachten en toetsvragen

In Jupyter Book kun je opdrachten en toetsvragen formuleren.

## Opdrachten

:::{exercise}
Gegeven is de bibliotheek-database.

Maak een top-5 van de leerlingen die in totaal het grootste bedrag aan boetes betaald hebben.

:::


## Toetsvragen

Deze toetsvragen kunnen de leerlingen gebruiken om na te gaan of ze de stof beheersen.
Er zijn verschillende soorten toetsvragen, hieronder een kleine selectie.

:::{mchoice} identificatie in een tabel
:correct: a

Hoe identificeer je de rijen en kolommen van een tabel in een relationele database?
In een tabel:

* geef je de kolommen namen en identificeer je de rijen met unieke keys
* geef je de rijen namen en identificeer je de kolommen met unieke keys
* identificeer je de rijen met unieke keys
* geef je de kolommen namen en nummer je de rijen altijd opeenvolgend
:::
   
:::{parsons} Volgorde in SQL

Zet de onderstaande onderdelen van de SQL opdracht in de juiste volgorde:

```SQL
SELECT  voornaam
,       achternaam
FROM leden
WHERE leden.voornaam = "Marie";
```

:::

:::{mchoice} samengestelde voorwaarde
:correct: a,c,d

Bekijk de volgende SQL query:

```SQL
SELECT voornaam, achternaam
FROM leerlingen
WHERE <voorwaarde> ;

```

Het is de bedoeling om alle leerlingen uit de 6e klas: 6a of 6b te selecteren.
Welke van de volgende mogelijkheden zijn juist als `<voorwaarde>`?

* `klas = '6a' OR klas = '6b'`
* `klas = '6a' OR '6b`
* `klas IN ('6a', '6b')`
* `klas LIKE '6_'`
* geen van deze mogelijkheden

:::

:::{mchoice} NULL in SQL
:correct: c

In SQL staat NULL voor:

* het getal 0
* de lege string, ''
* een ontbrekende waarde (leeg veld)
* een lege rij

:::


:::{parsons} Volgorde in SQL

Zet de onderstaande onderdelen van de SQL opdracht in de juiste volgorde.
(Laat de `JOIN` 1 positie inspringen.)

```SQL
SELECT voornaam, tussenvoegsel as tv, achternaam, boete
FROM leerlingen
     JOIN uitleningen ON leerlingen.llnr = uitleningen.llnr
WHERE boete > 3.50
ORDER BY achternaam
LIMIT 10;
```
:::
