<!DOCTYPE html>
<html lang="ro">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>BIG-MIC - Var Traditional</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f5f5f5;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            overflow: hidden;
        }

        /* Containerele pentru carte */
        .book {
            width: 80vw;
            height: 90vh;
            display: flex;
            flex-direction: row;
            perspective: 1500px; /* Efectul de adâncire pentru carte */
        }

        .book-page {
            width: 50%;
            height: 100%;
            background-color: #fff;
            border: 2px solid #ddd;
            transition: transform 1s;
            transform-origin: left;
            display: flex;
            justify-content: center;
            align-items: center;
            font-size: 1.5em;
            color: #333;
            padding: 20px;
            box-sizing: border-box;
        }

        .book-page.left {
            transform: rotateY(0deg);
        }

        .book-page.right {
            transform: rotateY(180deg);
        }

        .page-content {
            position: relative;
            z-index: 2;
        }

        .btn {
            position: absolute;
            top: 50%;
            left: 0;
            right: 0;
            width: 100%;
            padding: 10px;
            text-align: center;
            background-color: #8d6e63;
            color: white;
            font-size: 1.2em;
            cursor: pointer;
            transition: background-color 0.3s;
        }

        .btn:hover {
            background-color: #4e342e;
        }

        /* Ascunderea paginii când se întoarce */
        .book-page.turn {
            transform: rotateY(180deg);
        }
    </style>
</head>
<body>
    <div class="book">
        <div class="book-page left">
            <div class="page-content">
                <h2>Despre Noi</h2>
                <p>Suntem o fabrica traditionala de producere a varului bulgare si pasta, dedicata calitatii si autenticitatii.</p>
                <p>Varul nostru bulgare este obtinut traditional in cuptor pe lemne, iar varul pasta este perfect pentru aplicatii versatile.</p>
                <button class="btn" onclick="flipPage('left')">Urmeaza</button>
            </div>
        </div>
        <div class="book-page right">
            <div class="page-content">
                <h2>Produse</h2>
                <ul>
                    <li>Var Bulgare - Ideal pentru constructii, dezinfectat fantani, corectarea Ph sol, curatat si dezinfectat cotete animale, reducerea igrasiei, tratarea deseurilor periculoase, obtinut traditional in cuptor pe lemne.</li>
                    <li>Var Pasta - Perfect pentru varuitul locuintei, varuitul pomilor, fresca bisericeasca.</li>
                </ul>
                <button class="btn" onclick="flipPage('right')">Inapoi</button>
            </div>
        </div>
    </div>

    <script>
        function flipPage(side) {
            const leftPage = document.querySelector('.book-page.left');
            const rightPage = document.querySelector('.book-page.right');
            
            if (side === 'left') {
                leftPage.classList.add('turn');
                rightPage.classList.remove('turn');
            } else if (side === 'right') {
                rightPage.classList.add('turn');
                leftPage.classList.remove('turn');
            }
        }
    </script>
</body>
</html>
