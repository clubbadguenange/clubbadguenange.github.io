---
layout: default
title: Accueil
---

<html lang="fr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>{{ page.title }} | Association de Badminton</title>
    <link rel="stylesheet" href="/assets/styles.css">
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