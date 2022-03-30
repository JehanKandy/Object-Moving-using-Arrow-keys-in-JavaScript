# Object-Moving-using-Arrow-keys-in-JavaScript
Object Moving using Arrow keys in JavaScript
    <br><br>
    <b>Code Explane</b>
    <br>

in index.html <br>

        <!DOCTYPE html>
        <html lang="en">
        <head>
            <meta charset="UTF-8">
            <meta http-equiv="X-UA-Compatible" content="IE=edge">
            <meta name="viewport" content="width=device-width, initial-scale=1.0">
            <title>Ball Moving</title>
            <link rel="stylesheet" href="style.css">
        </head>
        <body>
            <div class="circle"></div>
            <script src="moving.js"></script>
        </body>
        </html>


**************************************************************




in here, <br>
I create a div class for circle, because in here I am going to moving a circle <br>
and also I call for moving.js javascript file to this project


********************************************************


<b><u>in moving.js file</u></b>


       let circle = document.querySelector('.circle');
       let moveBy = 50;

        window.addEventListener('load', () =>{
            circle.style.position = 'absolute';
            circle.style.left = 0;
            circle.style.top = 0;
        });

        window.addEventListener('keyup', (x) =>{
            switch(x.key){
                case "ArrowLeft":
                    circle.style.left = parseInt(circle.style.left) - moveBy + 'px'
                    break;
                case "ArrowRight":
                    circle.style.left = parseInt(circle.style.left) + moveBy + 'px'
                    break;
                case "ArrowUp":
                    circle.style.top = parseInt(circle.style.top) - moveBy + 'px'
                    break;
                case "ArrowDown":
                    circle.style.top = parseInt(circle.style.top) + moveBy + 'px'
            }

        });

