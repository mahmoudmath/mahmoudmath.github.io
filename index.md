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
            background: linear-gradient(135deg, #f8f9fa 0%, #e9ecef 100%);
            min-height: 100vh;
        }
        
        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 20px;
        }
        
        /* Header académique */
        .header {
            background: linear-gradient(135deg, #0056b3, #003d82);
            color: white;
            padding: 40px;
            border-radius: 15px;
            margin-bottom: 40px;
            text-align: center;
            box-shadow: 0 5px 20px rgba(0, 86, 179, 0.2);
        }
        
        .header h1 {
            font-size: 2.8em;
            margin-bottom: 15px;
        }
        
        .header p {
            font-size: 1.3em;
            opacity: 0.9;
        }
        
        .university-badge {
            display: inline-block;
            background: rgba(255, 255, 255, 0.2);
            padding: 10px 25px;
            border-radius: 30px;
            margin-top: 15px;
            font-weight: 500;
        }
        
        /* Navigation */
        .nav {
            display: flex;
            justify-content: center;
            flex-wrap: wrap;
            gap: 15px;
            margin-bottom: 40px;
            padding: 20px;
            background: white;
            border-radius: 12px;
            box-shadow: 0 3px 15px rgba(0,0,0,0.08);
        }
        
        .nav a {
            text-decoration: none;
            color: #0056b3;
            padding: 12px 25px;
            border-radius: 8px;
            font-weight: 600;
            transition: all 0.3s;
            border: 2px solid transparent;
        }
        
        .nav a:hover {
            background: #0056b3;
            color: white;
            border-color: #0056b3;
            transform: translateY(-2px);
        }
        
        /* Grid des cartes */
        .grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
            gap: 25px;
            margin: 40px 0;
        }
        
        .card {
            background: white;
            padding: 30px;
            border-radius: 12px;
            box-shadow: 0 5px 20px rgba(0,0,0,0.1);
            transition: all 0.3s ease;
            position: relative;
            overflow: hidden;
        }
        
        .card:hover {
            transform: translateY(-10px);
            box-shadow: 0 15px 30px rgba(0,0,0,0.15);
        }
        
        .card::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 5px;
        }
        
        .card-cours::before { background: #0056b3; }
        .card-td::before { background: #28a745; }
        .card-examens::before { background: #ffc107; }
        .card-contact::before { background: #dc3545; }
        
        .card h2 {
            color: #333;
            margin-bottom: 15px;
            font-size: 1.5em;
        }
        
        .card ul {
            list-style: none;
            margin: 20px 0;
        }
        
        .card li {
            padding: 8px 0;
            border-bottom: 1px solid #eee;
            position: relative;
            padding-left: 25px;
        }
        
        .card li::before {
            content: '✓';
            position: absolute;
            left: 0;
            color: #0056b3;
            font-weight: bold;
        }
        
        .btn {
            display: inline-block;
            padding: 12px 25px;
            background: linear-gradient(135deg, #0056b3, #007bff);
            color: white;
            text-decoration: none;
            border-radius: 8px;
            font-weight: 600;
            margin-top: 20px;
            transition: all 0.3s;
            border: none;
            cursor: pointer;
        }
        
        .btn:hover {
            background: linear-gradient(135deg, #004494, #0056b3);
            transform: translateY(-2px);
            box-shadow: 0 5px 15px rgba(0, 86, 179, 0.3);
        }
        
        /* Section actualités */
        .news {
            background: white;
            padding: 30px;
            border-radius: 12px;
            margin: 40px 0;
            box-shadow: 0 5px 20px rgba(0,0,0,0.1);
            border-left: 5px solid #0056b3;
        }
        
        .news h2 {
            color: #0056b3;
            margin-bottom: 20px;
            display: flex;
            align-items: center;
            gap: 10px;
        }
        
        /* Footer */
        .footer {
            margin-top: 60px;
            padding-top: 30px;
            border-top: 1px solid #ddd;
            text-align: center;
            color: #666;
        }
        
        .footer-links {
            display: flex;
            justify-content: center;
            gap: 30px;
            margin: 20px 0;
            flex-wrap: wrap;
        }
        
        .footer a {
            color: #0056b3;
            text-decoration: none;
        }
        
        /* Responsive */
        @media (max-width: 768px) {
            .header h1 { font-size: 2em; }
            .header p { font-size: 1.1em; }
            .nav { flex-direction: column; align-items: center; }
            .nav a { width: 100%; text-align: center; }
        }
    </style>
</head>
<body>
    <div class="container">
        <!-- En-tête académique -->
        <header class="header">
            <h1>🎓 Cours de Mathématiques</h1>
            <p>Faculté des Sciences et Techniques de Fès</p>
            <div class="university-badge">
                Université Sidi Mohamed Ben Abdellah (USMBA)
            </div>
        </header>
        
        <!-- Navigation -->
        <nav class="nav">
            <a href="/">Accueil</a>
            <a href="/cours/">Cours Magistraux</a>
            <a href="/td/">Travaux Dirigés</a>
            <a href="/examens/">Examens & Annales</a>
            <a href="/contact/">Contact</a>
        </nav>
        
        <!-- Grid des cartes -->
        <div class="grid">
            <div class="card card-cours">
                <h2>📘 Cours Magistraux</h2>
                <p>Supports de cours complets et détaillés pour tous les modules.</p>
                <ul>
                    <li>Analyse Réelle I & II</li>
                    <li>Algèbre Linéaire I & II</li>
                    <li>Probabilités et Statistiques</li>
                    <li>Analyse Complexe</li>
                    <li>Topologie</li>
                </ul>
                <a href="/cours/" class="btn">Accéder aux cours →</a>
            </div>
            
            <div class="card card-td">
                <h2>📝 Travaux Dirigés</h2>
                <p>Séries d'exercices corrigés et méthodes de résolution.</p>
                <ul>
                    <li>Séries hebdomadaires</li>
                    <li>Corrigés détaillés</li>
                    <li>Méthodologie</li>
                    <li>Exercices complémentaires</li>
                </ul>
                <a href="/td/" class="btn">Voir les TD →</a>
            </div>
            
            <div class="card card-examens">
                <h2>📊 Examens & Annales</h2>
                <p>Sujets et corrigés des années précédentes.</p>
                <ul>
                    <li>Contrôles continus</li>
                    <li>Examens semestriels</li>
                    <li>Corrigés types</li>
                    <li>Conseils de préparation</li>
                </ul>
                <a href="/examens/" class="btn">Consulter les examens →</a>
            </div>
            
            <div class="card card-contact">
                <h2>👨‍🏫 Contact & Informations</h2>
                <p>Coordonnées et informations pratiques.</p>
                <ul>
                    <li>Bureau : Bâtiment C, Bureau 210</li>
                    <li>Email : mahmoud.math@usmba.ac.ma</li>
                    <li>Permanence : Lundi & Jeudi, 14h-16h</li>
                    <li>Site FST : www.fstf.ump.ma</li>
                </ul>
                <a href="/contact/" class="btn">Nous contacter →</a>
            </div>
        </div>
        
        <!-- Actualités -->
        <section class="news">
            <h2>📅 Actualités Pédagogiques - Février 2025</h2>
            <ul>
                <li><strong>✅ Nouveaux supports :</strong> Cours d'Analyse 1 mis à jour</li>
                <li><strong>✅ TD ajoutés :</strong> Séries de Probabilités 1 à 3 disponibles</li>
                <li><strong>🔄 En cours :</strong> Numérisation des annales 2020-2024</li>
                <li><strong>📅 Prochainement :</strong> Forum de questions en ligne pour étudiants</li>
                <li><strong>📚 Bibliothèque :</strong> Nouveaux ouvrages référencés</li>
            </ul>
        </section>
        
        <!-- Modules -->
        <section class="news">
            <h2>🎯 Modules d'Enseignement 2024-2025</h2>
            <div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(250px, 1fr)); gap: 20px; margin-top: 20px;">
                <div>
                    <h3 style="color: #0056b3; margin-bottom: 10px;">Licence 1</h3>
                    <ul>
                        <li>MATH 101 - Analyse Réelle I (6cr)</li>
                        <li>MATH 102 - Algèbre Linéaire I (6cr)</li>
                        <li>MATH 103 - Méthodes Mathématiques (3cr)</li>
                    </ul>
                </div>
                <div>
                    <h3 style="color: #28a745; margin-bottom: 10px;">Licence 2</h3>
                    <ul>
                        <li>MATH 201 - Analyse Réelle II (6cr)</li>
                        <li>MATH 202 - Algèbre Linéaire II (6cr)</li>
                        <li>MATH 203 - Probabilités Élémentaires (3cr)</li>
                    </ul>
                </div>
                <div>
                    <h3 style="color: #ffc107; margin-bottom: 10px;">Licence 3</h3>
                    <ul>
                        <li>MATH 301 - Analyse Complexe (6cr)</li>
                        <li>MATH 302 - Topologie (6cr)</li>
                        <li>MATH 303 - Statistiques Inférentielles (6cr)</li>
                    </ul>
                </div>
            </div>
        </section>
        
        <!-- Footer -->
        <footer class="footer">
            <div class="footer-links">
                <a href="http://www.fstf.ump.ma" target="_blank">Site officiel FST Fès</a>
                <a href="https://www.usmba.ac.ma" target="_blank">Portail USMBA</a>
                <a href="http://biblio.fstf.ump.ma" target="_blank">Bibliothèque numérique</a>
                <a href="http://edt.fstf.ump.ma" target="_blank">Emploi du temps</a>
            </div>
            <p>© 2025 Faculté des Sciences et Techniques de Fès - Université Sidi Mohamed Ben Abdellah</p>
            <p>Département de Mathématiques | Enseignant responsable : Pr. Mahmoud Math</p>
            <p style="margin-top: 20px; font-size: 0.9em; color: #888;">
                Dernière mise à jour : Février 2025 | Plateforme pédagogique dédiée à l'excellence académique
            </p>
        </footer>
    </div>
</body>
</html>
