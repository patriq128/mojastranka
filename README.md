<!DOCTYPE html>
<html lang="sk">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Osobná stránka - PAtRiq</title>
    <style>
        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f0f2f5;
            color: #333;
        }
        header {
            background: linear-gradient(to right, #4CAF50, #2E7D32);
            color: white;
            padding: 2em 0;
            text-align: center;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
        }
        header h1 {
            margin: 0;
            font-size: 2.5em;
        }
        nav {
            text-align: center;
            margin: 1em 0;
        }
        nav button {
            background-color: #4CAF50;
            color: white;
            border: none;
            padding: 0.5em 1em;
            margin: 0 0.5em;
            border-radius: 4px;
            cursor: pointer;
            font-size: 1em;
        }
        nav button:hover {
            background-color: #388E3C;
        }
        section {
            display: none;
            padding: 2em;
            max-width: 900px;
            margin: 2em auto;
            background-color: white;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
            border-radius: 8px;
        }
        section.active {
            display: block;
        }
        h2 {
            color: #4CAF50;
            border-bottom: 2px solid #4CAF50;
            padding-bottom: 0.5em;
        }
        ul {
            list-style-type: none;
            padding: 0;
        }
        ul li {
            background: #e8f5e9;
            margin: 0.5em 0;
            padding: 0.5em;
            border-radius: 4px;
        }
        .contact a {
            color: #2E7D32;
            text-decoration: none;
            font-weight: bold;
        }
        .contact a:hover {
            text-decoration: underline;
        }
        footer {
            text-align: center;
            padding: 1em 0;
            background-color: #333;
            color: white;
            position: fixed;
            width: 100%;
            bottom: 0;
            box-shadow: 0 -4px 8px rgba(0, 0, 0, 0.2);
        }
        @media (max-width: 600px) {
            header, section {
                padding: 1em;
            }
            header h1 {
                font-size: 2em;
            }
        }
    </style>
</head>
<body>
    <header>
        <h1>Vitajte na mojej osobnej stránke!</h1>
    </header>
    <nav>
        <button onclick="showSection('about')">O mne</button>
        <button onclick="showSection('interests')">Záujmy</button>
        <button onclick="showSection('contact')">Kontakt</button>
    </nav>
    <section id="about" class="active">
        <h2>O mne</h2>
        <p>Ahoj, volám sa PAtRiq. Som nadšenec technológií a rád sa venujem najnovším trendom a inováciám v tejto oblasti.</p>
    </section>
    <section id="interests">
        <h2>Záujmy</h2>
        <p>Medzi moje hlavné záujmy patrí:</p>
        <ul>
            <li>Technológie</li>
            <li>Gadgety</li>
            <li>Programovanie</li>
            <li>Startupy</li>
        </ul>
    </section>
    <section id="contact">
        <h2>Kontakt</h2>
        <p>Sleduj ma na Instagrame: <a href="https://www.instagram.com/patri_kamin128" target="_blank">@patri_kamin128</a></p>
    </section>
    <footer>
        <p>&copy; 2024 PAtRiq. Všetky práva vyhradené.</p>
    </footer>
    <script>
        function showSection(id) {
            const sections = document.querySelectorAll('section');
            sections.forEach(section => {
                section.classList.remove('active');
            });
            document.getElementById(id).classList.add('active');
        }
    </script>
</body>
</html>

