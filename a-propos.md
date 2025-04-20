---
layout: default
title: À Propos de Nous
permalink: /a-propos/
---

<!DOCTYPE html>
<html lang="fr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>{{ page.title }} | Association de Badminton</title>
    <style>
        /* Styles spécifiques à la page À propos */
        .about-section {
            padding: 80px 0;
        }
        
        .about-content {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 50px;
            align-items: center;
        }
        
        .about-image {
            border-radius: 10px;
            overflow: hidden;
            box-shadow: 0 10px 30px rgba(0,0,0,0.1);
        }
        
        .about-image img {
            width: 100%;
            height: auto;
            display: block;
        }
        
        .about-text h2 {
            font-size: 36px;
            margin-bottom: 20px;
            color: var(--gray-dark);
        }
        
        .about-text p {
            margin-bottom: 20px;
            font-size: 16px;
            line-height: 1.8;
        }
        
        .team-section {
            padding: 80px 0;
            background-color: var(--gray-light);
        }
        
        .team-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 30px;
            margin-top: 50px;
        }
        
        .team-member {
            background-color: white;
            border-radius: 10px;
            overflow: hidden;
            box-shadow: 0 5px 15px rgba(0,0,0,0.05);
            text-align: center;
        }
        
        .member-image {
            height: 250px;
            background-color: var(--pink-light);
            display: flex;
            align-items: center;
            justify-content: center;
            color: white;
            font-size: 24px;
            font-weight: 700;
        }
        
        .member-info {
            padding: 20px;
        }
        
        .member-name {
            font-size: 20px;
            margin-bottom: 5px;
        }
        
        .member-title {
            color: var(--pink-dark);
            font-size: 14px;
            margin-bottom: 15px;
        }
        
        .member-bio {
            font-size: 14px;
            color: #666;
        }
        
        @media (max-width: 768px) {
            .about-content {
                grid-template-columns: 1fr;
            }
            
            .about-image {
                margin-bottom: 30px;
            }
        }
    </style>
</head>
<body>
    <!-- En-tête et autres composants du layout par défaut -->
    
    <!-- Section À propos -->
    <section class="about-section">
        <div class="container">
            <div class="about-content">
                <div class="about-image">
                    <img src="{{ site.baseurl }}/assets/images/about-image.jpg" alt="Joueurs de badminton en action">
                </div>
                <div class="about-text">
                    <h2>Notre Histoire</h2>
                    <p>Fondée en 2010, notre Association de Badminton a évolué d'un petit groupe de passionnés à une communauté florissante de joueurs de tous niveaux et de tous horizons.</p>
                    <p>Notre mission est de promouvoir le sport du badminton, de fournir des formations de qualité et des opportunités de compétition, et de construire une communauté solidaire pour les joueurs de tous âges et de toutes capacités.</p>
                    <p>Au fil des années, nous avons organisé de nombreux tournois, ateliers et événements sociaux qui ont contribué à connecter les amateurs de badminton et à élever ce sport dans notre région.</p>
                    <p>Nos installations comprennent 8 courts professionnels, une zone d'entraînement et un salon de club où les membres peuvent se détendre et socialiser après les matchs.</p>
                </div>
            </div>
        </div>
    </section>
    
    <!-- Section Équipe -->
    <section class="team-section">
        <div class="container">
            <div class="section-title">
                <h3>Rencontrez Notre Équipe</h3>
                <div class="divider"></div>
            </div>
            <div class="team-grid">
                <div class="team-member">
                    <div class="member-image">Jean Dupont</div>
                    <div class="member-info">
                        <h4 class="member-name">Jean Dupont</h4>
                        <div class="member-title">Président</div>
                        <p class="member-bio">Ancien joueur national avec plus de 20 ans d'expérience dans ce sport. Jean dirige notre association depuis 2015.</p>
                    </div>
                </div>
                <div class="team-member">
                    <div class="member-image">Sophie Martin</div>
                    <div class="member-info">
                        <h4 class="member-name">Sophie Martin</h4>
                        <div class="member-title">Entraîneur Principal</div>
                        <p class="member-bio">Coach certifiée internationale qui a formé des champions juniors. Sophie se concentre sur le développement des joueurs de tous niveaux.</p>
                    </div>
                </div>
                <div class="team-member">
                    <div class="member-image">Michel Thomas</div>
                    <div class="member-info">
                        <h4 class="member-name">Michel Thomas</h4>
                        <div class="member-title">Coordinateur d'Événements</div>
                        <p class="member-bio">Michel assure le bon déroulement de nos tournois et événements et crée des activités engageantes pour nos membres.</p>
                    </div>
                </div>
                <div class="team-member">
                    <div class="member-image">Léa Chen</div>
                    <div class="member-info">
                        <h4 class="member-name">Léa Chen</h4>
                        <div class="member-title">Responsable des Adhésions</div>
                        <p class="member-bio">Léa gère toutes les demandes d'adhésion et s'assure que les nouveaux membres se sentent bienvenus dans notre communauté.</p>
                    </div>
                </div>
            </div>
        </div>
    </section>
    
    <!-- Pied de page du layout par défaut -->
</body>
</html>