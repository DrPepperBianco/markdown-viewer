---
title: Frontmatter YAML Test
author: Rattunde
date: 2026-07-10
tags:
  - markdown
  - viewer
  - frontmatter
draft: false
---

# Frontmatter (YAML) — Test

> Feature: **content → „Display yaml/toml frontmatter"** (PR #281)

**So testen:**

1. Option **aus**: Der `---`-Block oben wird **entfernt** (nicht angezeigt), aber
   der Tab-Titel wird auf „Frontmatter YAML Test" gesetzt.
2. Option **an**: Der Block oben erscheint **als YAML-Codeblock** am Anfang des
   Dokuments.

Danach kommt normaler Inhalt:

## Abschnitt

Etwas Fließtext, damit man den Übergang vom Frontmatter zum Inhalt sieht.

- Punkt eins
- Punkt zwei
