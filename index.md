---
layout: default
title: Accueil
---

<!DOCTYPE html>
<html lang="fr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>{{ page.title }} | Association de Badminton</title>
    <style>
        /* Styles globaux */
        :root {
            --pink-light: #ff99cc;
            --pink-dark: #e6388b;
            --gray-light: #f5f5f5;
            --gray-dark: #333333;
        }
        
        body {
            font-family: 'Montserrat', sans-serif;
            margin: 0;
            padding: 0;
            color: var(--gray-dark);
            background-color: #ffffff;
            line-height: 1.6;
        }
        
        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 20px;
        }
        
        /* Styles d'en-tête */
        header {
            background-color: #ffffff;
            box-shadow: 0 2px 10px rgba(0,0,0,0.1);
            position: sticky;
            top: 0;
            z-index: 100;
        }
        
        .header-container {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 15px 0;
        }
        
        .logo {
            display: flex;
            align-items: center;
        }
        
        .logo img {
            height: 50px;
            margin-right: 10px;
        }
        
        .logo h1 {
            font-size: 24px;
            font-weight: 700;
            margin: 0;
            color: var(--pink-dark);
        }
        
        nav ul {
            display: flex;
            list-style: none;
            margin: 0;
            padding: 0;
        }
        
        nav ul li {
            margin-left: 30px;
        }
        
        nav ul li a {
            text-decoration: none;
            color: var(--gray-dark);
            font-weight: 600;
            text-transform: uppercase;
            font-size: 14px;
            transition: color 0.3s ease;
        }
        
        nav ul li a:hover {
            color: var(--pink-dark);
        }
        
        /* Section Héro */
        .hero {
            background: linear-gradient(135deg, var(--pink-light), var(--pink-dark));
            color: white;
            padding: 80px 0;
            text-align: center;
        }
        
        .hero h2 {
            font-size: 48px;
            margin-bottom: 20px;
            font-weight: 800;
            text-shadow: 2px 2px 4px rgba(0,0,0,0.2);
        }
        
        .hero p {
            font-size: 18px;
            max-width: 700px;
            margin: 0 auto 30px;
        }
        
        .btn {
            display: inline-block;
            background-color: white;
            color: var(--pink-dark);
            padding: 12px 30px;
            border-radius: 30px;
            text-decoration: none;
            font-weight: 600;
            transition: all 0.3s ease;
            text-transform: uppercase;
            letter-spacing: 1px;
            font-size: 14px;
        }
        
        .btn:hover {
            transform: translateY(-3px);
            box-shadow: 0 10px 20px rgba(0,0,0,0.1);
        }
        
        /* Section Caractéristiques */
        .features {
            padding: 80px 0;
            background-color: var(--gray-light);
        }
        
        .section-title {
            text-align: center;
            margin-bottom: 60px;
        }
        
        .section-title h3 {
            font-size: 36px;
            color: var(--gray-dark);
            margin-bottom: 20px;
        }
        
        .section-title .divider {
            height: 4px;
            width: 70px;
            background-color: var(--pink-dark);
            margin: 0 auto;
        }
        
        .features-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 30px;
        }
        
        .feature-card {
            background-color: white;
            border-radius: 10px;
            padding: 30px;
            box-shadow: 0 5px 15px rgba(0,0,0,0.05);
            transition: transform 0.3s ease;
            text-align: center;
        }
        
        .feature-card:hover {
            transform: translateY(-10px);
        }
        
        .feature-icon {
            font-size: 48px;
            color: var(--pink-dark);
            margin-bottom: 20px;
        }
        
        .feature-card h4 {
            font-size: 20px;
            margin-bottom: 15px;
            color: var(--gray-dark);
        }
        
        /* Section Événements */
        .events {
            padding: 80px 0;
        }
        
        .events-list {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 30px;
        }
        
        .event-card {
            border-radius: 10px;
            overflow: hidden;
            box-shadow: 0 5px 15px rgba(0,0,0,0.05);
            transition: transform 0.3s ease;
        }
        
        .event-card:hover {
            transform: translateY(-10px);
        }
        
        .event-image {
            height: 200px;
            background-color: var(--pink-light);
            display: flex;
            align-items: center;
            justify-content: center;
            color: white;
            font-size: 24px;
            font-weight: 700;
        }
        
        .event-details {
            padding: 20px;
            background-color: white;
        }
        
        .event-date {
            color: var(--pink-dark);
            font-weight: 600;
            margin-bottom: 10px;
            font-size: 14px;
        }
        
        .event-title {
            font-size: 20px;
            margin-bottom: 10px;
        }
        
        .event-description {
            color: #666;
            margin-bottom: 20px;
            font-size: 14px;
        }
        
        /* Pied de page */
        footer {
            background-color: var(--gray-dark);
            color: white;
            padding: 60px 0 30px;
        }
        
        .footer-content {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 40px;
            margin-bottom: 40px;
        }
        
        .footer-column h4 {
            font-size: 18px;
            margin-bottom: 20px;
            color: white;
            position: relative;
            padding-bottom: 10px;
        }
        
        .footer-column h4::after {
            content: '';
            position: absolute;
            left: 0;
            bottom: 0;
            width: 40px;
            height: 3px;
            background-color: var(--pink-dark);
        }
        
        .footer-column ul {
            list-style: none;
            padding: 0;
            margin: 0;
        }
        
        .footer-column ul li {
            margin-bottom: 10px;
        }
        
        .footer-column ul li a {
            color: #bbb;
            text-decoration: none;
            transition: color 0.3s ease;
        }
        
        .footer-column ul li a:hover {
            color: var(--pink-light);
        }
        
        .social-icons {
            display: flex;
            gap: 15px;
        }
        
        .social-icons a {
            color: white;
            font-size: 18px;
            transition: color 0.3s ease;
        }
        
        .social-icons a:hover {
            color: var(--pink-light);
        }
        
        .footer-bottom {
            text-align: center;
            padding-top: 30px;
            border-top: 1px solid rgba(255,255,255,0.1);
            font-size: 14px;
            color: #999;
        }
        
        /* Responsive */
        @media (max-width: 768px) {
            .header-container {
                flex-direction: column;
                text-align: center;
            }
            
            .logo {
                margin-bottom: 20px;
                justify-content: center;
            }
            
            nav ul {
                flex-direction: column;
                align-items: center;
            }
            
            nav ul li {
                margin: 10px 0;
            }
            
            .hero h2 {
                font-size: 36px;
            }
        }
    </style>
</head>
<body>
    <!-- En-tête -->
    <header>
        <div class="container header-container">
            <div class="logo">
                <img src="{{ site.baseurl }}/assets/images/logo.png" alt="Logo Association de Badminton">
                <h1>Association de Badminton</h1>
            </div>
            <nav>
                <ul>
                    <li><a href="{{ site.baseurl }}/">Accueil</a></li>
                    <li><a href="{{ site.baseurl }}/a-propos">À propos</a></li>
                    <li><a href="{{ site.baseurl }}/evenements">Événements</a></li>
                    <li><a href="{{ site.baseurl }}/adhesion">Adhésion</a></li>
                    <li><a href="{{ site.baseurl }}/galerie">Galerie</a></li>
                    <li><a href="{{ site.baseurl }}/contact">Contact</a></li>
                </ul>
            </nav>
        </div>
    </header>

    <!-- Section Héro -->
    <section class="hero">
        <div class="container">
            <h2>Bienvenue à Notre Association de Badminton</h2>
            <p>Rejoignez notre communauté dynamique de passionnés de badminton. Que vous soyez débutant ou expert, nous avons quelque chose pour vous !</p>
            <a href="{{ site.baseurl }}/adhesion" class="btn">Adhérer Maintenant</a>
        </div>
    </section>

    <!-- Section Caractéristiques -->
    <section class="features">
        <div class="container">
            <div class="section-title">
                <h3>Nos Services</h3>
                <div class="divider"></div>
            </div>
            <div class="features-grid">
                <div class="feature-card">
                    <div class="feature-icon">🏸</div>
                    <h4>Coaching Professionnel</h4>
                    <p>Apprenez avec des entraîneurs expérimentés qui vous aideront à améliorer vos compétences et votre technique.</p>
                </div>
                <div class="feature-card">
                    <div class="feature-icon">🏆</div>
                    <h4>Tournois Réguliers</h4>
                    <p>Participez à nos tournois mensuels et relevez des défis face à d'autres joueurs.</p>
                </div>
                <div class="feature-card">
                    <div class="feature-icon">👥</div>
                    <h4>Événements Communautaires</h4>
                    <p>Rejoignez nos rencontres sociales et faites de nouvelles connaissances qui partagent votre passion pour le badminton.</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Section Événements -->
    <section class="events">
        <div class="container">
            <div class="section-title">
                <h3>Événements À Venir</h3>
                <div class="divider"></div>
            </div>
            <div class="events-list">
                <div class="event-card">
                    <div class="event-image">Tournoi d'Été</div>
                    <div class="event-details">
                        <div class="event-date">15 juin 2025</div>
                        <h4 class="event-title">Tournoi Annuel d'Été</h4>
                        <p class="event-description">Rejoignez-nous pour notre plus grand tournoi de l'année avec des joueurs de tous niveaux.</p>
                        <a href="{{ site.baseurl }}/evenements/tournoi-ete" class="btn">En Savoir Plus</a>
                    </div>
                </div>
                <div class="event-card">
                    <div class="event-image">Atelier Débutants</div>
                    <div class="event-details">
                        <div class="event-date">10 mai 2025</div>
                        <h4 class="event-title">Atelier pour Débutants</h4>
                        <p class="event-description">Un atelier spécial pour les nouveaux venus qui souhaitent apprendre les bases du badminton.</p>
                        <a href="{{ site.baseurl }}/evenements/atelier-debutants" class="btn">En Savoir Plus</a>
                    </div>
                </div>
                <div class="event-card">
                    <div class="event-image">Match Amical</div>
                    <div class="event-details">
                        <div class="event-date">25 mai 2025</div>
                        <h4 class="event-title">Soirée Matchs Amicaux</h4>
                        <p class="event-description">Un événement décontracté où les membres peuvent jouer des matchs amicaux et améliorer leurs compétences.</p>
                        <a href="{{ site.baseurl }}/evenements/match-amical" class="btn">En Savoir Plus</a>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Pied de page -->
    <footer>
        <div class="container">
            <div class="footer-content">
                <div class="footer-column">
                    <h4>À Propos de Nous</h4>
                    <p>Nous sommes une communauté de passionnés de badminton dédiée à promouvoir ce sport et à offrir une plateforme pour les joueurs de tous niveaux.</p>
                </div>
                <div class="footer-column">
                    <h4>Liens Rapides</h4>
                    <ul>
                        <li><a href="{{ site.baseurl }}/">Accueil</a></li>
                        <li><a href="{{ site.baseurl }}/a-propos">À propos</a></li>
                        <li><a href="{{ site.baseurl }}/evenements">Événements</a></li>
                        <li><a href="{{ site.baseurl }}/adhesion">Adhésion</a></li>
                        <li><a href="{{ site.baseurl }}/galerie">Galerie</a></li>
                        <li><a href="{{ site.baseurl }}/contact">Contact</a></li>
                    </ul>
                </div>
                <div class="footer-column">
                    <h4>Contactez-nous</h4>
                    <p>123 Avenue du Sport<br>
                    Ville du Badminton, VB 12345<br>
                    info@associationbadminton.org<br>
                    (123) 456-7890</p>
                </div>
                <div class="footer-column">
                    <h4>Suivez-nous</h4>
                    <div class="social-icons">
                        <a href="#" title="Facebook">FB</a>
                        <a href="#" title="Twitter">TW</a>
                        <a href="#" title="Instagram">IG</a>
                        <a href="#" title="YouTube">YT</a>
                    </div>
                </div>
            </div>
            <div class="footer-bottom">
                <p>&copy; 2025 Association de Badminton. Tous droits réservés.</p>
            </div>
        </div>
    </footer>
</body>
</html>