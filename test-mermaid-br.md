# Mermaid `<br>` in Node-Labels — Test

> Feature: **content → „Mermaid diagrams"** muss **an** sein (PR #289).

**So testen:** In den Knoten unten stehen `<br>`-Umbrüche. Erwartung: Die Labels
werden **mehrzeilig** dargestellt (Zeilenumbruch sichtbar), nicht als eine lange
Zeile und nicht mit sichtbarem Text „\<br\>".

```mermaid
flowchart TD
    A["Erste Zeile<br>Zweite Zeile<br>Dritte Zeile"] --> B["Einzeiliger Knoten"]
    B --> C["Noch ein<br>mehrzeiliger<br>Knoten"]
    C --> D["Ende"]
```

## Zweites Diagramm (Sequenz, zur Kontrolle)

```mermaid
sequenceDiagram
    participant U as User
    participant E as Extension
    U->>E: Markdown öffnen
    E-->>U: gerendertes HTML
```

---

**Hinweis:** Falls die `<br>`-Umbrüche im ersten Diagramm *nicht* greifen und die
Labels einzeilig bleiben, könnte dafür Mermaids `securityLevel: 'loose'` nötig
sein — das haben wir aus Sicherheitsgründen bewusst **nicht** übernommen (nur den
CSS-Fix). Dann müssten wir das separat abwägen.
