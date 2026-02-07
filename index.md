<!DOCTYPE html>
<html lang="fr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Cours de Mathématiques - FST Fès</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Arial, sans-serif;
        }
        
        body {
            background: #f8f9fa;
            color: #333;
            line-height: 1.6;
        }
        
        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 20px;
        }
        
        /* Header unique */
        .site-header {
            background: linear-gradient(135deg, #0056b3, #003d82);
            color: white;
            padding: 40px;
            border-radius: 15px;
            margin-bottom: 30px;
            text-align: center;
        }
        
        .site-header h1 {
            font-size: 2.5em;
            margin-bottom: 10px;
        }
        
        .site-header .subtitle {
            font-size: 1.2em;
            opacity: 0.9;
            margin-bottom: 10px;
        }
        
        .university {
            background: rgba(255, 255, 255, 0.2);
            padding: 8px 20px;
            border-radius: 20px;
            display: inline-block;
            font-size: 0.9em;
        }
        
        /* Navigation */
        .main-nav {
            display: flex;
            justify-content: center;
            gap: 15px;
            margin: 30px 0;
            flex-wrap: wrap;
        }
        
        .nav-btn {
            background: white;
            color: #0056b3;
            padding: 12px 25px;
            border-radius: 8px;
            text-decoration: none;
            font-weight: 600;
            border: 2px solid #0056b3;
            transition: all 0.3s;
        }
        
        .nav-btn:hover {
            background: #0056b3;
            color: white;
        }
        
        /* Sections */
        .section {
            background: white;
            padding: 30px;
            border-radius: 12px;
            margin-bottom: 25px;
            box-shadow: 0 3px 10px rgba(0,0,0,0.08);
        }
        
        .section h2 {
            color: #0056b3;
            margin-bottom: 20px;
            border-bottom: 2px solid #0056b3;
            padding-bottom: 10px;
        }
        
        /* Grid pour les cartes */
        .features-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
            gap: 25px;
            margin: 30px 0;
        }
        
        .feature-card {
            background: white;
            padding: 25px;
            border-radius: 10px;
            box-shadow: 0 5px 15px rgba(0,0,0,0.1);
            border-top: 5px solid #0056b3;
        }
        
        .feature-card h3 {
            color: #0056b3;
            margin-bottom: 15px;
            display: flex;
            align-items: center;
            gap: 10px;
        }
        
        .feature-list {
            list-style: none;
            margin: 15px 0;
        }
        
        .feature-list li {
            padding: 8px 0;
            border-bottom: 1px solid #eee;
            padding-left: 25px;
            position: relative;
        }
        
        .feature-list li:before {
            content: '✓';
            position: absolute;
            left: 0;
            color: #28a745;
            font-weight: bold;
        }
        
        .btn {
            display: inline-block;
            background: #0056b3;
            color: white;
            padding: 10px 20px;
            border-radius: 6px;
            text-decoration: none;
            margin-top: 15px;
            font-weight: 500;
            transition: background 0.3s;
        }
        
        .btn:hover {
            background: #004494;
        }
        
        /* Table */
        .modules-table {
            width: 100%;
            border-collapse: collapse;
            margin: 20px 0;
        }
        
        .modules-table th {
            background: #0056b3;
            color: white;
            padding: 15px;
            text-align: left;
        }
        
        .modules-table td {
            padding: 12px 15px;
            border-bottom: 1px solid #eee;
        }
        
        .modules-table tr:hover {
            background: #f8f9fa;
        }
        
        /* Footer */
        .site-footer {
            margin-top: 50px;
            padding-top: 25px;
            border-top: 1px solid #ddd;
            text-align: center;
            color: #666;
        }
        
        .footer-links {
            display: flex;
            justify-content: center;
            gap: 25px;
            margin: 20px 0;
            flex-wrap: wrap;
        }
        
        .footer-links a {
            color: #0056b3;
            text-decoration: none;
        }
        
        /* Responsive */
        @media (max-width: 768px) {
            .site-header h1 { font-size: 2em; }
            .main-nav { flex-direction: column; align-items: center; }
            .nav-btn { width: 100%; text-align: center; }
            .features-grid { grid-template-columns: 1fr; }
        }
    </style>
</head>
<body>
    <div class="container">
        <!-- EN-TÊTE UNIQUE -->
        <header class="site-header">
            <h1>🎓 Cours de Mathématiques</h1>
            <div class="subtitle">Faculté des Sciences et Techniques de Fès</div>
            <div class="university">Université Sidi Mohamed Ben Abdellah (USMBA)</div>
        </header>
        
        <!-- Navigation -->
        <nav class="main-nav">
            <a href="/" class="nav-btn">Accueil</a>
            <a href="/cours/" class="nav-btn">Cours</a>
            <a href="/td/" class="nav-btn">Travaux Dirigés</a>
            <a href="/examens/" class="nav-btn">Examens</a>
            <a href="/contact/" class="nav-btn">Contact</a>
        </nav>
        
        <!-- Introduction -->
        <section class="section">
            <h2>📚 Plateforme Pédagogique Officielle</h2>
            <p>Bienvenue sur la plateforme numérique du <strong>Département de Mathématiques</strong> de la Faculté des Sciences et Techniques de Fès.</p>
            <p>Cette plateforme centralise l'ensemble des ressources pédagogiques destinées aux étudiants des filières mathématiques.</p>
        </section>
        
        <!-- Cartes de fonctionnalités -->
        <div class="features-grid">
            <div class="feature-card">
                <h3>📘 Cours Magistraux</h3>
                <p>Supports de cours complets et structurés :</p>
                <ul class="feature-list">
                    <li>Analyse Réelle I & II</li>
                    <li>Algèbre Linéaire I & II</li>
                    <li>Probabilités et Statistiques</li>
                    <li>Analyse Complexe</li>
                </ul>
                <a href="/cours/" class="btn">Accéder aux cours →</a>
            </div>
            
            <div class="feature-card">
                <h3>📝 Travaux Dirigés</h3>
                <p>Séries d'exercices et corrigés :</p>
                <ul class="feature-list">
                    <li>Séries hebdomadaires</li>
                    <li>Corrigés détaillés</li>
                    <li>Méthodologie de résolution</li>
                    <li>Exercices complémentaires</li>
                </ul>
                <a href="/td/" class="btn">Voir les TD →</a>
            </div>
            
            <div class="feature-card">
                <h3>📊 Examens & Annales</h3>
                <p>Ressources pour les révisions :</p>
                <ul class="feature-list">
                    <li>Contrôles continus</li>
                    <li>Examens semestriels</li>
                    <li>Corrigés types</li>
                    <li>Conseils de préparation</li>
                </ul>
                <a href="/examens/" class="btn">Consulter →</a>
            </div>
            
            <div class="feature-card">
                <h3>👨‍🏫 Contact & Infos</h3>
                <p>Informations pratiques :</p>
                <ul class="feature-list">
                    <li>Bureau : Bâtiment C, Bureau 210</li>
                    <li>Email : mahmoud.math@usmba.ac.ma</li>
                    <li>Permanence : Lundi & Jeudi</li>
                    <li>Site FST : www.fstf.ump.ma</li>
                </ul>
                <a href="/contact/" class="btn">Nous contacter →</a>
            </div>
        </div>
        
        <!-- Actualités -->
        <section class="section">
            <h2>📅 Actualités - Février 2025</h2>
            <ul class="feature-list">
                <li><strong>Nouveautés :</strong> Cours d'Analyse 1 mis à jour</li>
                <li><strong>Ajouts :</strong> TD de Probabilités disponibles</li>
                <li><strong>En cours :</strong> Numérisation des annales</li>
                <li><strong>Prochainement :</strong> Forum étudiant en ligne</li>
            </ul>
        </section>
        
        <!-- Modules -->
        <section class="section">
            <h2>🎯 Modules d'Enseignement 2024-2025</h2>
            <table class="modules-table">
                <thead>
                    <tr>
                        <th>Licence 1 (6 crédits)</th>
                        <th>Licence 2 (6 crédits)</th>
                        <th>Licence 3 (6 crédits)</th>
                    </tr>
                </thead>
                <tbody>
                    <tr>
                        <td>MATH 101 - Analyse Réelle I</td>
                        <td>MATH 201 - Analyse Réelle II</td>
                        <td>MATH 301 - Analyse Complexe</td>
                    </tr>
                    <tr>
                        <td>MATH 102 - Algèbre Linéaire I</td>
                        <td>MATH 202 - Algèbre Linéaire II</td>
                        <td>MATH 302 - Topologie</td>
                    </tr>
                    <tr>
                        <td>MATH 103 - Méthodes Mathématiques</td>
                        <td>MATH 203 - Probabilités Élémentaires</td>
                        <td>MATH 303 - Statistiques Inférentielles</td>
                    </tr>
                </tbody>
            </table>
        </section>
        
        <!-- Footer -->
        <footer class="site-footer">
            <div class="footer-links">
                <a href="http://www.fstf.ump.ma" target="_blank">Site FST Fès</a>
                <a href="https://www.usmba.ac.ma" target="_blank">Portail USMBA</a>
                <a href="http://biblio.fstf.ump.ma" target="_blank">Bibliothèque</a>
                <a href="http://edt.fstf.ump.ma" target="_blank">Emploi du temps</a>
            </div>
            <p>© 2025 Faculté des Sciences et Techniques de Fès - USMBA</p>
            <p>Département de Mathématiques | Enseignant : Pr. Mahmoud Math</p>
        </footer>
    </div>
</body>
</html>
