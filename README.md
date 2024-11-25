<!DOCTYPE html>
<html lang="de">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>HTW Saar Campus Orientierung</title>
  <link rel="stylesheet" href="style.css">
</head>
<body>
  <header>
    <h1>Willkommen am HTW Saar Campus Rotenbühl</h1>
    <nav>
      <ul>
        <li><a href="#mensa">Mensa</a></li>
        <li><a href="#drucker">Druckerräume</a></li>
        <li><a href="#kontakt">Kontakt & Termine</a></li>
      </ul>
    </nav>
  </header>

  <main>
    <section id="mensa">
      <h2>Mensa</h2>
      <p>Die Mensa befindet sich im Kellergeschoss (KG). Sie bietet eine Außenterrasse und ist über den Eingang Ost zugänglich.</p>
    </section>

    <section id="drucker">
      <h2>Druckerräume</h2>
      <p>Druckerräume finden Sie in Raum A-K-08 und B-1-15. Weitere Informationen sind im IT-Service verfügbar.</p>
    </section>

    <section id="map">
      <h2>Kartenansicht</h2>
      <img src="assets/campus-plan.png" alt="Campus Rotenbühl Plan">
    </section>

    <section id="kontakt">
      <h2>Kontakt & Termine</h2>
      <p>Buchen Sie einen Termin mit uns über unser Online-Formular:</p>
      <div id="calendly">
        <iframe 
          src="https://calendly.com/your-calendly-link" 
          width="100%" 
          height="600" 
          frameborder="0">
        </iframe>
      </div>
    </section>
  </main>

  <footer>
    <p>&copy; 2024 HTW Saar - Campus Rotenbühl Orientierung</p>
  </footer>
  
  <script src="script.js"></script>
</body>
</html>

body {
  font-family: Arial, sans-serif;
  line-height: 1.6;
  margin: 0;
  padding: 0;
  color: #333;
  background-color: #f4f4f4;
}

header {
  background: #333;
  color: #fff;
  padding: 1rem 0;
  text-align: center;
}

header h1 {
  margin: 0;
}

nav ul {
  display: flex;
  justify-content: center;
  list-style: none;
  padding: 0;
}

nav ul li {
  margin: 0 15px;
}

nav ul li a {
  color: #fff;
  text-decoration: none;
  font-weight: bold;
}

main {
  padding: 20px;
}

main section {
  margin: 20px 0;
  background: #fff;
  padding: 20px;
  border-radius: 8px;
  box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
}

footer {
  text-align: center;
  padding: 10px;
  background: #333;
  color: #fff;
}


