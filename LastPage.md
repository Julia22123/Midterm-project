[Home Page](README.md) | [Animals](FavAnimals.md) | [What I am studying](major.md) |
[Colors](FavColor.md) | [Seasons](FavorteSeasons.md) 
---
### A code I have fixed

It's not the most *effective* way to do it 

but this was how I solved the  code problem

and **it works** following the [Fizz Buzz game](https://en.wikipedia.org/wiki/Fizz_buzz) rules



    <!DOCTYPE html>
    <!--Julia A last edited 10/14/22-->
    <html>
    <head>
    <meta charset="UTF-8">
    <title>Fizz Buzz</title>
    <script>

    function fizzbuzz() {
        var display = document.getElementById('display');
        var displayHTML = "";
        var result3 = 0;
        var result5 = 0;
        var result15 = 0;
        var Fizzbuzz = false;
        for (i = 1; i < 101; i++) {
            result3 = i%3;
            result5 = i%5;
            result15 = i%15;
            if (result15 == 0) {
                displayHTML += "<p>FizzBuzz</p>";
                Fizzbuzz = true;
            }
            if (Fizzbuzz === false) {
                if (result3 == 0) {
                    displayHTML += "<p>Fizz</p>";
                    Fizzbuzz = true;
                }
                if (result5 == 0) {
                    displayHTML += "<p>Buzz</p>";
                    Fizzbuzz = true;
                }
                if (Fizzbuzz === false) {
                    displayHTML += "<p>" + i + "</p>";
                }
            }
            Fizzbuzz = false;
        }
        display.innerHTML = displayHTML
    }

    </script>

    </head>

    <body onload="fizzbuzz()">
    <div id="display">

    </div>
    </body>

    </html>