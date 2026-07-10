# Grid Tables — Test

> Feature: **compiler → markdown-it → „support for pandoc grid_tables"** (PR #233)
> Voraussetzung: Compiler = **markdown-it** (nicht marked/remark).

**So testen:** Option **aus** → der Block unten bleibt roher Text (Plus/Striche
sichtbar). Option **an** → er wird als **Tabelle** gerendert (inkl. mehrzeiliger
Zellen und Listen in Zellen, was normale Markdown-Tabellen nicht können).

## Einfaches Grid Table

+---------------+---------------+
| Frucht        | Preis         |
+===============+===============+
| Bananen       | 1,34 €        |
+---------------+---------------+
| Orangen       | 2,10 €        |
+---------------+---------------+

## Grid Table mit mehrzeiligen Zellen und Listen

+---------------+---------------+----------------------+
| Frucht        | Preis         | Vorteile             |
+===============+===============+======================+
| Bananen       | 1,34 €        | - eigene Verpackung  |
|               |               | - kräftige Farbe     |
+---------------+---------------+----------------------+
| Orangen       | 2,10 €        | - gegen Skorbut      |
|               |               | - schmackhaft und    |
|               |               |   sehr saftig        |
+---------------+---------------+----------------------+

## Zum Vergleich: normale Markdown-Tabelle (geht immer)

| Frucht  | Preis  |
| :------ | -----: |
| Bananen | 1,34 € |
| Orangen | 2,10 € |
