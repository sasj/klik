# 2: p5js

Tijdens de lessen gebruiken we ook de website [p5.js referentie](https://p5js.org/reference/) voor meer informatie over functies en methoden.


### Ga naar editor.p5js.org 
Maak een account aan. Hiermee kunnen we de sketches opslaan

**Belangrijk:** dat je je werk regelmatig opslaat.

### Editor Overzicht
Overzicht van de editor, wat zien we allemaal? 

### Basisinstelling
- **Setup** Functie om je sketch te initialiseren 
- **Draw** Functie waar we continu updaten 
- **CreateCanvas** Hiermee maak je een tekengebied aan
- **Background** Stel de achtergrondkleur in

### Belangrijke Tekens
- **Komma ,**: Scheidt waarden in functie-argumenten.
- **Ronde Haken ()**: Worden gebruikt om functies aan te roepen.
- **Vierkante Haken []**: Worden gebruikt voor arrays.
- **Puntkomma ;**: Beëindigt een statement.

### Kleuren
Je kunt kleuren gebruiken in je tekeningen met functies zoals `fill()` en `background()`.


### Aan de Slag!
Wat hebben we daarvoor nodig? 

1. **Een Ellips Tekenen**:
    ```javascript
    ellipse(200, 200, 100, 100);
    ```

2. **Gebruik Muispositie**:
    ```javascript
    ellipse(mouseX, mouseY, 100, 100);
    ```

3. **Spoor Zonder Achtergrond**:
    Verwijder `background()` om een spoor achter te laten.

4. **Alleen Tekenen Bij Muisklik**:
    ```javascript
    if (mouseIsPressed) {
        ellipse(mouseX, mouseY, 50, 50);
    }
    ```

5. **Kleur op Muispositie**:
    ```javascript
    fill(mouseX, mouseY, 255);
    noStroke();
    ```



