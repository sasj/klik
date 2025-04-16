# 3: Knop maken

Met deze code maak je een ellips die als knop fungeert. Wanneer je binnen de ellips klikt, verandert de achtergrondkleur en schakelt tussen twee kleuren.


### Een Knop Maken

De basis. Wat hebben wij nodig?

- [MousePressed](https://p5js.org/reference/p5/mousePressed/)

```javascript
function setup() {
  createCanvas(400, 400);
}

function draw() {
  background(220);
  ellipse(width/2, height/2, 50, 50);
}

function mousePressed(){

}
```


### Achtergrondkleur Veranderen

We maken een variabele aan voor de achtergrond

```javascript
let bgColor = 0;

+

background(bgColor);
```

### Kleuren:

'#FFA0CC'

→ We moeten de positie van de ellips weten en controleren.

```javascript
let posX = 200;
let posY = 200;
let dim = 50;

+
ellipse(posX, posY, dim, dim);
```

→ Controleer waar de muispositie is.
[Referentie voor `dist`](https://p5js.org/reference/p5/dist/)

```javascript
let d = dist(mouseX, mouseY, posX, posY);
```

Welke waarde geeft `d`?

```javascript
console.log(d);
```

```javascript
if (d < dim/2) {
    bgColor = '#FF00CC';
} else {
    bgColor = '#AA00CC';
}
```


### alleen veranderen als we op de knop drukken

```javascript
// Voeg een variabele toe bovenaan het programma
let buttonState = false; 

// volgende veranderen we

function mousePressed() {
  let d = dist(mouseX, mouseY, posX, posY);
  
  if (d < dim/2) {
    buttonState = !buttonState;
    
    if (buttonState) {
      bgColor = '#FF00CC';
    } else {
      bgColor = '#AA00CC';
    }
    
  }
}

```



### Al klaar? 
Kan je nog een button maken? Wat heb je daarvoor nodig? 


