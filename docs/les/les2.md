# 2: 



### Editor Overzicht
1. **Dark Mode en Opslaan**: Zorg ervoor dat je de dark mode inschakelt en je werk regelmatig opslaat.

### Basisinstelling
1. **Setup & Draw**: Deze functies worden gebruikt om je sketch te initialiseren en continu te updaten.
2. **CreateCanvas**: Hiermee maak je een tekengebied aan.
3. **Background**: Stel de achtergrondkleur in.

### Belangrijke Tekens
- **Komma (,)**: Scheidt waarden in functie-argumenten.
- **Ronde Haken ()**: Worden gebruikt om functies aan te roepen.
- **Vierkante Haken []**: Worden gebruikt voor arrays.
- **Puntkomma (;)**: Beëindigt een statement.

### Kleuren
Je kunt kleuren gebruiken in je tekeningen met functies zoals `fill()` en `background()`.

### Referentie
Gebruik de [p5.js referentie](https://p5js.org/reference/) voor meer informatie over functies en methoden.

### Aan de Slag!
1. **Een Ellips Tekenen**:
    ```jsx
    ellipse(200, 200, 100, 100);
    ```

2. **Gebruik Muispositie**:
    ```jsx
    ellipse(mouseX, mouseY, 100, 100);
    ```

3. **Spoor Zonder Achtergrond**:
    Verwijder `background()` om een spoor achter te laten.

4. **Alleen Tekenen Bij Muisklik**:
    ```jsx
    if (mouseIsPressed) {
        ellipse(mouseX, mouseY, 50, 50);
    }
    ```

5. **Kleur op Muispositie**:
    ```jsx
    fill(mouseX, mouseY, 255);
    noStroke();
    ```

### MousePressed Functie
De `mousePressed` functie wordt uitgevoerd wanneer de muis wordt ingedrukt en kan worden gebruikt om acties uit te voeren.

Voorbeeld:
```jsx
let shape = 0;

function mousePressed() {
    if (shape === 0) {
        rect(mouseX, mouseY, 50, 50);
        shape = 1;
    } else {
        ellipse(mouseX, mouseY, 50, 50);
        shape = 0;
    }
}
```

### Extra Tips
- **Globale Waarden**: Je kunt globale variabelen gebruiken om de staat van je sketch bij te houden.
- **Voorbeelden**: Bekijk de voorbeelden in de p5.js referentie voor meer ideeën en inspiratie.

Als je vragen hebt of hulp nodig hebt met specifieke code, laat het me weten!