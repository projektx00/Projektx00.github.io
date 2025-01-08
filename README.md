<!DOCTYPE html>
<html lang="de">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Website mit Navigation und FAQ</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
        }
        header {
            background-color: #0073e6;
            color: white;
            padding: 10px 20px;
            text-align: center;
        }
        .navbar {
            display: flex;
            justify-content: center;
            background-color: #004080;
            padding: 10px 0;
        }
        .navbar a {
            color: white;
            text-decoration: none;
            padding: 10px 15px;
            transition: background-color 0.3s;
        }
        .navbar a:hover {
            background-color: #0059b3;
            border-radius: 5px;
        }
        .content {
            padding: 20px;
            text-align: center;
        }
        iframe {
            margin: auto;
            display: block;
        }
        footer {
            background-color: #004080;
            color: white;
            text-align: center;
            padding: 10px 0;
            position: fixed;
            bottom: 0;
            width: 100%;
        }
        @media (max-width: 768px) {
            .navbar {
                flex-direction: column;
                align-items: center;
            }
            .navbar a {
                margin: 5px 0;
            }
        }
        .faq-section {
            max-width: 800px;
            margin: 50px auto;
            padding: 20px;
            background-color: #fff;
            border-radius: 10px;
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
        }
        .faq-header {
            text-align: center;
            margin-bottom: 20px;
        }
        .faq-header h1 {
            margin: 0;
            font-size: 2rem;
            color: #007BFF;
        }
        .faq-item {
            border-bottom: 1px solid #ddd;
            padding: 10px 0;
        }
        .faq-item:last-child {
            border-bottom: none;
        }
        .faq-question {
            display: flex;
            justify-content: space-between;
            align-items: center;
            cursor: pointer;
            font-size: 1.1rem;
            padding: 10px;
            transition: background-color 0.3s;
        }
        .faq-question:hover {
            background-color: #f0f8ff;
        }
        .faq-icon {
            font-size: 1.5rem;
            color: #007BFF;
            transition: transform 0.3s;
        }
        .faq-answer {
            display: none;
            padding: 10px 20px;
            font-size: 1rem;
            color: #555;
            line-height: 1.6;
            border-left: 4px solid #007BFF;
            background-color: #f8f9fa;
            border-radius: 5px;
        }
        .faq-answer.open {
            display: block;
        }
        .faq-icon.rotate {
            transform: rotate(180deg);
        }
        .section {
            text-align: center;
            margin-bottom: 20px;
        }
        .section ul {
            list-style: none;
            padding: 0;
        }
        .section ul li {
            margin: 5px 0;
        }
        .map-link {
            display: inline-block;
            margin-top: 10px;
            color: #007BFF;
            text-decoration: none;
        }
        .map-link:hover {
            text-decoration: underline;
        }
    </style>
    <script>
        document.addEventListener("DOMContentLoaded", () => {
            const faqItems = document.querySelectorAll('.faq-item');
            faqItems.forEach(item => {
                const question = item.querySelector('.faq-question');
                const answer = item.querySelector('.faq-answer');
                const icon = item.querySelector('.faq-icon');
                question.addEventListener('click', () => {
                    const isOpen = answer.classList.toggle('open');
                    icon.classList.toggle('rotate', isOpen);
                });
            });
        });
    </script>
</head>
<body>
    <header>
        <h1>Willkommen am Campus Rotenbühl - htw saar</h1>
    </header>
    <nav class="navbar">
        <a href="#gebäudea">Gebäude A</a>
        <a href="#gebäudeb">Gebäude B</a>
        <a href="#faq">FAQ</a>
        <a href="#standort">Standort</a>
        <a href="#kontakt">Kontakt</a>
    </nav>
    <iframe width="560" height="315" 
    src="https://www.youtube.com/embed/zLOsksQYCkc" 
    title="YouTube video player" 
    frameborder="0" 
    allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" 
    allowfullscreen>
    </iframe>
    <div class="section">
        <h2>Wichtige Bereiche:</h2>
        <ul>
            <li><strong>Gebäude A:</strong> Bibliothek </li>
            <li><strong>Gebäude B:</strong> Sekretariate </li>
            <li><strong>Gebäude C:</strong> Auditorium </li>
            <li><strong>Gebäude D:</strong> Senatsaal </li>
            <li><strong>Gebäude E:</strong> IT-Labore </li>
            <li><strong>Gebäude F:</strong> ESG </li>
            <li><strong>Mensa:</strong> Mittagessen und Snacks</li>
            <li><strong>Innenhof & Aussenterrasse</strong> </li>
        </ul>
    </div>
    <div class="content">
        <section id="gebäudea">
            <h2>Gebäude A</h2>
            <p><strong>KG:</strong> Bibliothek</p>
            <p>Praxisreferat</p>
            <p>Fachschaft</p>
            <p>International Office</p>
            <p><strong>EG:</strong> IT-Service</p>
        </section>
        <section id="gebäudeb">
            <h2>Gebäude B</h2>
            <p><strong>EG:</strong> Empfang</p>
            <p>Konferenzraum</p>
            <p>Info-Corner</p>
            <p><strong>OG1:</strong> Sekretariat</p>
            <p>Besprechungsraum</p>
            <p><strong>OG2:</strong> IT-Labor</p>
        </section>
        <section id="faq">
            <div class="faq-section">
                <div class="faq-header">
                    <h1>Häufig gestellte Fragen</h1>
                </div>
                <div class="faq-item">
                    <div class="faq-question">
                        <span>Wo befindet sich die Mensa auf dem Campus?</span>
                        <span class="faq-icon">▼</span>
                    </div>
                    <div class="faq-answer">Die Mensa befindet sich im Gebäude C im Kellergeschoss.</div>
                </div>
                <div class="faq-item">
                    <div class="faq-question">
                        <span>Was sind die Öffnungszeiten der Mensa?</span>
                        <span class="faq-icon">▼</span>
                    </div>
                    <div class="faq-answer">Die Mensa ist von 7:00 Uhr bis 14:45 Uhr geöffnet. An Wochenenden geschlossen.</div>
                </div>
                <div class="faq-item">
                    <div class="faq-question">
                        <span>Wo finde ich die Druckerräume auf dem Campus?</span>
                        <span class="faq-icon">▼</span>
                    </div>
                    <div class="faq-answer">Die Druckerräume befinden sich in den Gebäuden C und D im Erdgeschoss.</div>
                </div>
                <div class="faq-item">
                    <div class="faq-question">
                        <span>Was kostet das Drucken und Kopieren?</span>
                        <span class="faq-icon">▼</span>
                    </div>
                    <div class="faq-answer">Die Kosten liegen bei 0,10 € pro Seite für Schwarz-Weiß und 0,20 € pro Seite für Farbkopien.</div>
                </div>
            </div>
        </section>
        <section id="standort">
            <h2>Standort HTW Saar Campus Rotenbühl</h2>
            <iframe 
                src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d2689.329495621813!2d7.0131173!3d49.2434243!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x4795b699fbe34679%3A0x14f2a1681f6f62b1!2sHochschule%20f%C3%BCr%20Technik%20und%20Wirtschaft%20Campus%20Rotenb%C3%BChl%20-%20WIWI!5e0!3m2!1sen!2sde!4v1694190735111!5m2!1sen!2sde" 
                width="100%" 
                height="450" 
                style="border:0;" 
                allowfullscreen="" 
                loading="lazy">
            </iframe>
        </section>
        <div class="section">
            <h2>Campusplan</h2>
            <p>Hier finden Sie den vollständigen Orientierungsplan:</p>
            <a class="map-link" href="https://www.htwsaar.de/wiwi/campusleben/campusvorstellung/dateien/orientierungsplan_crb_072017.pdf" target="_blank">
                Campusplan als PDF anzeigen
            </a>
        </div>
        <section id="kontakt">
            <h2>Kontakt</h2>
            <p><strong>Adresse:</strong> Waldhausweg 14, 66123 Saarbrücken</p>
            <p><strong>Telefon:</strong> +49 681 58 67 512</p>
            <p><strong>E-Mail:</strong> info@htwsaar.de</p>
        </section>
    </div>
    <footer>
        © 2024 HTW Saar - Campus Rotenbühl
    </footer>
</body>
</html>
