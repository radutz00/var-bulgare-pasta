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
        }
        header {
            background-color: #8d6e63;
            color: white;
            padding: 20px;
            text-align: center;
        }
        nav {
            background-color: #d7ccc8;
            display: flex;
            justify-content: center;
            padding: 10px;
            flex-direction: column;
        }
        nav a {
            margin: 5px 0;
            text-decoration: none;
            color: #4e342e;
        }
        .dropdown {
            position: relative; /* Asigură că submeniul va fi poziționat corect */
        }
        .dropdown-content {
            display: none;
            background-color: #f1f1f1;
            min-width: 160px;
            padding: 10px;
            box-shadow: 0px 8px 16px rgba(0, 0, 0, 0.2);
            position: absolute;
            top: 100%;
            left: 0;
            opacity: 0; /* Inițial, submeniul va fi invizibil */
            transform: translateY(-20px); /* Submeniul începe mai sus */
            transition: opacity 0.3s ease, transform 0.3s ease; /* Efecte de tranziție */
        }
        .dropdown:hover .dropdown-content {
            display: block;
            opacity: 1; /* Submeniul devine vizibil */
            transform: translateY(0); /* Submeniul se va mișca la locul său */
        }
        section {
            padding: 20px;
        }
        footer {
            background-color: #8d6e63;
            color: white;
            text-align: center;
            padding: 10px;
            position: fixed;
            bottom: 0;
            width: 100%;
        }
    </style>
</head>
<body>
    <header>
        <h1>BIG-MIC - Var Traditional</h1>
    </header>
    <nav>
        <div class="dropdown">
            <a href="#">Despre Noi</a>
            <div class="dropdown-content">
                <a href="#despre">Despre Firma</a>
                <a href="#produse">Produse</a>
                <a href="#recenzii">Recenzii</a>
                <a href="#contact">Contact</a>
            </div>
        </div>
    </nav>
    <div class="hero">
        <h2>Calitate si Traditie in Productia de Var</h2>
    </div>
    <section id="despre">
        <h2>Despre Noi</h2>
        <p>Suntem o fabrica traditionala de producere a varului bulgare si pasta, dedicata calitatii si autenticitatii.</p>
        <p>Varul nostru bulgare este obtinut traditional in cuptor pe lemne, iar varul pasta este perfect pentru aplicatii versatile.</p>
    </section>
    <section id="produse">
        <h2>Produse</h2>
        <ul>
            <li>Var Bulgare - Ideal pentru constructii, dezinfectat fantani, corectarea Ph sol, curatat si dezinfectat cotete animale, reducerea igrasiei, tratarea deseurilor periculoase, obtinut traditional in cuptor pe lemne.</li>
            <li>Var Pasta - Perfect pentru varuitul locuintei, varuitul pomilor, fresca bisericeasca.</li>
        </ul>
    </section>
    <section id="recenzii">
        <h2>Recenzii</h2>
        <p><strong>Ion Popescu:</strong> „Varul de la BIG-MIC este de o calitate exceptionala! L-am folosit pentru renovarea casei si sunt foarte multumit de rezultate.”</p>
        <p><strong>Maria Ionescu:</strong> „Recomand cu incredere varul pastă! Este usor de folosit si are o textura fina.”</p>
    </section>
    <section id="contact">
        <h2>Contact</h2>
        <p>Email: radutzu2009@yahoo.com</p>
        <p>Telefon: 0758280873</p>
    </section>
    <footer>
        <p>&copy; 2024 BIG-MIC. Toate drepturile rezervate.</p>
    </footer>
</body>
</html>
