<!DOCTYPE html>
<html lang="fr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Cours de Mathématiques - FST Fès</title>

    <style>
        :root {
            --primary: #0056b3;
            --primary-dark: #003d82;
            --success: #28a745;
            --warning: #ffc107;
            --danger: #dc3545;
            --bg-light: #f8f9fa;
            --shadow-soft: 0 3px 10px rgba(0,0,0,0.05);
            --shadow-medium: 0 5px 20px rgba(0,0,0,0.1);
            --radius: 12px;
            --transition: all 0.3s ease;
            --font-main: 'Segoe UI', Arial, sans-serif;
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: var(--font-main);
        }

        body {
            background: linear-gradient(135deg, var(--bg-light), #e9ecef);
            min-height: 100vh;
            color: #333;
        }

        .container {
            max-width: 1200px;
            margin: auto;
            padding: 20px;
        }

        /* ===== HEADER ===== */
        .header {
            background: linear-gradient(135deg, var(--primary), var(--primary-dark));
            color: white;
            padding: 40px;
            border-radius: 15px;
            text-align: center;
            box-shadow: 0 5px 20px rgba(0,86,179,.2);
            margin-bottom: 30px;
        }

        .header h1 { font-size: 2.5em; margin-bottom: 10px; }
        .header h2 { font-size: 1.3em; opacity: .9; }

        .university-badge {
            margin-top: 15px;
            padding: 8px 20px;
            border-radius: 30px;
            background: rgba(255,255,255,.2);
            display: inline-block;
            font-size: .9em;
        }

        /* ===== NAV ===== */
        .nav {
            display: flex;
            gap: 15px;
            justify-content: center;
            flex-wrap: wrap;
            padding: 20px;
            background: white;
            border-radius: var(--radius);
            box-shadow: var(--shadow-soft);
            margin-bottom: 30px;
        }

        .nav a {
            text-decoration: none;
            color: var(--primary);
            font-weight: 600;
            padding: 10px 20px;
            border-radius: 8px;
            transition: var(--transition);
        }

        .nav a:hover {
            background: var(--primary);
            color: white;
        }

        /* ===== SECTIONS COMMUNES ===== */
        .section {
            background: white;
            padding: 25px;
            border-radius: var(--radius);
            margin: 30px 0;
            box-shadow: var(--shadow-soft);
            border-left: 5px solid var(--primary);
        }

        .section h2,
        .section h3 {
            color: var(--primary);
            margin-bottom: 15px;
        }

        /* ===== GRID & CARDS ===== */
        .grid {
            display: grid;
            gap: 25px;
            margin: 40px 0;
            grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
        }

        .card {
            background: white;
            padding: 25px;
            border-radius: var(--radius);
            box-shadow: var(--shadow-medium);
            position: relative;
            transition: var(--transition);
        }

        .card:hover {
            transform: translateY(-5px);
        }

        .card::before {
            content: "";
            position: absolute;
            top: 0;
            left: 0;
            height: 5px;
            width: 100%;
        }

        .card[data-color="primary"]::before { background: var(--primary); }
        .card[data-color="success"]::before { background: var(--success); }
        .card[data-color="warning"]::before { background: var(--warning); }
        .card[data-color="danger"]::before  { background: var(--danger); }

        .card ul {
            list-style: none;
            margin: 15px 0;
        }

        .card li {
            padding: 8px 0 8px 25px;
            border-bottom: 1px solid #eee;
            position: relative;
        }

        .card li::before {
            content: "✓";
            position: absolute;
            left: 0;
            color: var(--primary);
        }

        /* ===== BUTTON ===== */
        .btn {
            display: inline-block;
            margin-top: 15px;
            padding: 10px 20px;
            background: linear-gradient(135deg, var(--primary), #007bff);
            color: white;
            text-decoration: none;
            border-radius: 6px;
            font-weight: 600;
            transition: var(--transition);
        }

        .btn:hover {
            background: linear-gradient(135deg, #004494, var(--primary));
        }

        /* ===== TABLE ===== */
        .modules-table {
            width: 100%;
            border-collapse: collapse;
            margin-top: 15px;
        }

        .modules-table th {
            background: var(--primary);
            color: white;
            padding: 15px;
            text-align: left;
        }

        .modules-table td {
            padding: 12px 15px;
            border-bottom: 1px solid #eee;
        }

        .modules-table tr:hover {
            background: var(--bg-light);
        }

        /* ===== FOOTER ===== */
        .footer {
            margin-top: 50px;
            padding-top: 25px;
            border-top: 1px solid #ddd;
            text-align: center;
            font-size: .9em;
            color: #666;
        }

        .footer-links {
            display: flex;
            justify-content: center;
            gap: 25px;
            flex-wrap: wrap;
            margin-bottom: 15px;
        }

        .footer a {
            color: var(--primary);
            text-decoration: none;
        }

        /* ===== RESPONSIVE ===== */
        @media (max-width: 768px) {
            .header h1 { font-size: 2em; }
            .nav { flex-direction: column; }
        }
    </style>
</head>

<body>
<div class="container">

    <header class="header">
        <h1>🎓 Cours de Mathématiques</h1>
        <h2>Faculté des Sciences et Techniques de Fès</h2>
        <div class="university-badge">
            Université Sidi Mohamed Ben Abdellah (USMBA)
        </div>
    </header>

    <nav class="nav">
        <a href="/">Accueil</a>
        <a href="/cours/">Cours</a>
        <a href="/td/">TD</a>
        <a href="/examens/">Examens</a>
        <a href="/contact/">Contact</a>
    </nav>

    <section class="section">
        <h2>Plateforme Officielle d'Enseignement</h2>
        <p>Département de Mathématiques – FST Fès.</p>
        <p>Ressources pédagogiques complètes pour les étudiants en mathématiques.</p>
    </section>

    <div class="grid">
        <div class="card" data-color="primary">
            <h3>📘 Cours Magistraux</h3>
            <ul>
                <li>Analyse Réelle I & II</li>
                <li>Algèbre Linéaire I & II</li>
                <li>Analyse Complexe</li>
                <li>Topologie</li>
            </ul>
            <a href="/cours/" class="btn">Accéder</a>
        </div>

        <div class="card" data-color="success">
            <h3>📝 Travaux Dirigés</h3>
            <ul>
                <li>Séries corrigées</li>
                <li>Méthodologie</li>
                <li>Exercices supplémentaires</li>
            </ul>
            <a href="/td/" class="btn">Voir TD</a>
        </div>

        <div class="card" data-color="warning">
            <h3>📊 Examens</h3>
            <ul>
                <li>Contrôles</li>
                <li>Annales</li>
                <li>Corrigés types</li>
            </ul>
            <a href="/examens/" class="btn">Consulter</a>
        </div>

        <div class="card" data-color="danger">
            <h3>👨‍🏫 Contact</h3>
            <ul>
                <li>Bureau C-210</li>
                <li>mahmoud.math@usmba.ac.ma</li>
                <li>Lundi & Jeudi 14h–16h</li>
            </ul>
            <a href="/contact/" class="btn">Contact</a>
        </div>
    </div>

    <section class="section">
        <h3>🎯 Modules 2024–2025</h3>
        <table class="modules-table">
            <tr>
                <th>Licence 1</th>
                <th>Licence 2</th>
                <th>Licence 3</th>
            </tr>
            <tr>
                <td>Analyse Réelle I</td>
                <td>Analyse Réelle II</td>
                <td>Analyse Complexe</td>
            </tr>
            <tr>
                <td>Algèbre Linéaire I</td>
                <td>Algèbre Linéaire II</td>
                <td>Topologie</td>
            </tr>
        </table>
    </section>

    <footer class="footer">
        <div class="footer-links">
            <a href="https://www.usmba.ac.ma" target="_blank">USMBA</a>
            <a href="http://www.fstf.ump.ma" target="_blank">FST Fès</a>
        </div>
        <p>© 2025 FST Fès – Département de Mathématiques</p>
    </footer>

</div>
</body>
</html>
