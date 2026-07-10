# Copy-Button Test

Kurzer Fließtext davor. Unten drei Codeblöcke mit unterschiedlichen Sprachen —
jeder sollte oben rechts einen **Copy**-Button zeigen (wenn die Option `copy`
im Popup aktiviert ist).

## JavaScript

```javascript
function greet(name) {
  console.log(`Hallo, ${name}!`)
  return name.length
}
greet('Rattunde')
```

## Python

```python
def fib(n):
    a, b = 0, 1
    for _ in range(n):
        a, b = b, a + b
    return a

print([fib(i) for i in range(10)])
```

## Bash

```bash
#!/usr/bin/env bash
set -euo pipefail
for f in *.md; do
  echo "processing: $f"
done
```

## Lange Zeile (Wrap-Test)

```javascript
const url = 'https://example.com/api/v1/resource?param1=verylongvalue&param2=anotherlongvalue&param3=yetanotherlongvalue&param4=stillgoing&param5=almostdone&token=abcdef0123456789abcdef0123456789'
const config = { retries: 5, timeout: 30000, headers: { 'Authorization': 'Bearer sehr-langer-token-der-normalerweise-eine-horizontale-scrollleiste-erzeugen-wuerde' } }
```

## Code ohne Sprachangabe (Grenzfall)

```
Plain text ohne language-Klasse.
Prüfen, ob hier ein Button erscheint oder nicht.
```

Text danach — ende.
