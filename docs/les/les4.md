### GIF's Tonen en Veranderen met Toetsaanslagen

In deze les gaan we GIF's tonen en veranderen met behulp van toetsaanslagen. We gebruiken  twee GIF's in de code maar je kan er altijd meer toevoegen



#### Uitleg

1. **Preload**: Laad de GIF's vooraf in met de `preload` functie.
    ```javascript
    function preload() {
      gif0 = createImg("https://media.giphy.com/media/ebFG4jcnC1Ny8/giphy.gif");
      gif1 = createImg("https://media.giphy.com/media/HMSLfCl5BsXoQ/giphy.gif");
    }
    ```

2. **Setup**: Maak een canvas en verberg alle GIF's. Toon vervolgens de eerste GIF.
    ```javascript
    function setup() {
      createCanvas(400, 400);
      gif0.hide();
      gif1.hide();

      showThisGif = gif0.show();
    }
    ```

3. **Draw**: Teken de achtergrond en positioneer de huidige GIF in het midden van het canvas.
    ```javascript
    function draw() {
      background(220);

      showThisGif.position(
        width / 2 - showThisGif.width / 2,
        height / 2 - showThisGif.height / 2
      );
    }
    ```

4. **KeyTyped**: Verberg alle GIF's en toon de GIF die overeenkomt met de ingedrukte toets.
    ```javascript
    function keyTyped() {
      gif0.hide();
      gif1.hide();

      if (key === '2') {
        showThisGif = gif1.show();
      } else if (key === '1') {
        showThisGif = gif0.show();
      }
    }
    ```

