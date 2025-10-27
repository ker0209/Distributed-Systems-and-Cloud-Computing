
📘RAPPORT DE PROJET
Medifind – SIMPLIFIER ET OPTIMISER L'ACCÈS À L'INFORMATION SUR LA DISPONIBILITÉ ET LE PRIX DES MÉDICAMENTS
________________________________________
Université : ICT UNIVERSITY

Département : Génie logiciel

Cours : Systèmes distribués et cloud computing

Id cours : CS 4122

Titre du projet : Medifind – Plateforme digital multicanaux pour simplifier et optimiser l'accès à l'information sur la disponibilité et le prix des médicaments 

Étudiant : BOGNE FOUSSOM KERYAN MERVEIL

Matricule Étudiant : ICTU20241354

Supervisuer : Ing. Moune
Année universitaire : 2025–2026
________________________________________

I. Table des Matières
Résumé Exécutif
1.1 Objectif général du projet
1.2 Présentation de MediFind
1.3 Enjeux et valeur ajoutée
1.4 Publics cibles et bénéfices par acteur
Description et Portée du Problème
2.1 Contexte général du secteur pharmaceutique
2.2 Problématiques identifiées : Une analyse approfondie
2.3 Analyse des besoins des utilisateurs
2.4 Portée du projet et limitations de la phase I
2.5 Analyse de la concurrence et positionnement différentiel
Proposition de Solution : MediFind
3.1 Vision du projet
3.2 Principes de conception
3.3 Objectifs fonctionnels et non fonctionnels
3.4 Modèle économique et stratégie de partenariat
Architecture et Conception du Système
4.1 Vue d’ensemble de l’architecture
4.2 Description détaillée des microservices
4.3 Schéma fonctionnel et flux d’information
4.4 Sécurité, performance et interopérabilité
4.5 Gestion des données et modèle conceptuel
Technologies Proposées
5.1 Choix technologiques et justifications
5.2 Outils de développement, test et intégration
5.3 Stratégie de déploiement et configuration
5.4 Stratégie de sauvegarde et reprise après sinistre
Calendrier d’Activités et Jalons (Phase I — 12 Mois)
6.1 Étapes de développement détaillées
6.2 Méthodologie de gestion de projet
6.3 Indicateurs de performance et livrables
6.4 Analyse des risques et plan d'atténuation
Conclusion et Prochaines Étapes
7.1 Synthèse globale du projet
7.2 Perspectives d’évolution à moyen terme
7.3 Recommandations finales

II. Résumé Exécutif

1.1 Objectif général du projet
Le projet MediFind vise à résoudre une problématique quotidienne pour des millions de personnes : simplifier et optimiser l'accès à l'information sur la disponibilité et le prix des médicaments dans les pharmacies de proximité. Il s'agit de mettre fin à la recherche fastidieuse par téléphone ou par déplacement physique en offrant une solution numérique centralisée, fiable et intuitive. L'objectif ultime est de réduire le temps d'accès aux médicaments de plus de 70% et de favoriser une transparence du marché bénéfique au consommateur.

1.2 Présentation de MediFind
MediFind est une plateforme digitale multi-canaux qui se décline sous deux formes pour maximiser son accessibilité :
•	Application Web Responsive : Accessible via tout navigateur moderne sur ordinateur, tablette ou smartphone, sans nécessité de téléchargement.
•	Application Mobile Native : Développée avec le framework Flutter pour offrir une expérience performante et homogène sur iOS et Android à partir d'une base de code unique.
Publics cibles principaux :
•	Les Citoyens/Patients : Personnes cherchant un médicament spécifique, avec un besoin critique d'efficacité et de fiabilité.
•	Les Pharmacies Partenaires : Officines souhaitant digitaliser leur visibilité, attirer une nouvelle clientèle et optimiser la gestion des demandes sur leurs stocks.
•	Les Autorités Sanitaires : Acteurs publics qui pourront exploiter des données agrégées et anonymisées pour la veille épidémiologique, le suivi des pénuries ou l'analyse des flux géographiques de consommation.

1.3 Enjeux et valeur ajoutée
Enjeux : Dans un contexte urbain et semi-urbain, la recherche d'un médicament est souvent un parcours du combattant, générant du stress, une perte de temps et des coûts de transport superflus. Pour le pharmacien, la gestion des appels téléphoniques répétitifs est chronophage et peu efficiente.
Valeur ajoutée de MediFind :
•	Accessibilité & Gain de Temps : Centralisation de l'information en un point unique, accessible en quelques clics.
•	Fiabilité & Confiance : Mise à jour en temps quasi-réel des stocks via une interface dédiée pour les pharmaciens, garantissant l'exactitude de l'information.
•	Transparence Économique : La comparaison des prix entre pharmacies voisines permet aux utilisateurs de faire des choix éclairés et encourage une saine concurrence.
•	Efficacité Opérationnelle : Pour les pharmacies, réduction significative des interruptions de travail pour répondre aux demandes téléphoniques de disponibilité.
1.4 Publics cibles et bénéfices par acteur
•	Pour le Citoyen : Économie de temps et d'argent, réduction du stress, meilleur accès aux soins.
•	Pour le Pharmacien : Augmentation du trafic en officine, outil de gestion et d'analyse du stock, modernisation de l'image de marque.
•	Pour les Autorités : Outil de veille sanitaire et de pilotage du territoire, amélioration de l'efficacité du système de santé global.

III. Description et Portée du Problème

2.1 Contexte général
Le secteur pharmaceutique de détail, bien que régulé, reste fragmenté dans sa gestion de l'information. L'absence d'interconnexion numérique entre les pharmacies crée une asymétrie d'information préjudiciable au consommateur. Alors que la digitalisation touche la plupart des secteurs économiques, la recherche de médicaments en reste souvent à des méthodes archaïques.

2.2 Problématiques identifiées : Une analyse approfondie
•	Fragmentation de l'Information : Chaque pharmacie est un silo d'information. Aucune base de données centralisée ou fédérée n'existe pour offrir une vue unifiée des stocks.
•	Inefficacité des Canaux Traditionnels : La recherche par téléphone est aléatoire (ligne occupée, personnel indisponible) et le déplacement physique "au hasard" est un gaspillage de ressources.
•	Délai d'Information Critique : Dans des situations de besoin urgent (fièvre, douleur, traitement chronique oublié), le temps perdu dans la recherche peut avoir un impact direct sur le bien-être de l'individu.
•	Opacité des Prix : Les différences de prix, bien que réglementées, existent. Le consommateur n'a pas les moyens de les identifier facilement, ce qui l'empêche de réaliser des économies.

2.3 Analyse des besoins des utilisateurs
Une enquête qualitative préliminaire (entretiens avec 20 pharmaciens et 50 patients) a fait émerger les besoins suivants :
•	Pour l'Utilisateur Final :
o	Interface "minimaliste" : Saisir le nom du médicament et voir immédiatement les résultats autour de soi.
o	Filtres indispensables : par distance, prix, et disponibilité immédiate.
o	Informations contextuelles : horaires d'ouverture, numéro de téléphone, possibilité de réserver.
o	Confiance absolue dans la fiabilité des stocks affichés.
•	Pour le Pharmacien Partenaire :
o	Interface de gestion simple et rapide pour mettre à jour les stocks (via un portail web ou une application tablette).
o	Gain de temps net par rapport à la situation actuelle.
o	Retour sur investissement clair (augmentation du chiffre d'affaires).

2.4 Portée du projet et limitations de la phase I (MVP)
La Phase I (Minimum Viable Product) se concentre sur les fonctions essentielles de découverte et de localisation :
•	Inscription et authentification des utilisateurs et des pharmaciens.
•	Recherche géolocalisée de médicaments par nom.
•	Affichage des pharmacies avec le médicament en stock, leur prix, leur distance et leurs coordonnées.
•	Calcul d'itinéraire via intégration Google Maps.
•	Interface d'administration basique pour les pharmaciens (gestion du stock).
•	Hors portée pour le MVP : Commande en ligne, paiement électronique, livraison à domicile, gestion des ordonnances dématérialisées, module de recommandation.

2.5 Analyse de la concurrence et positionnement différentiel
Il existe quelques applications similaires sur le marché, souvent locales et peu connues. Le positionnement de MediFind repose sur :
•	Une Approche Centrée sur l'Expérience Utilisateur : Interface plus intuitive et plus rapide que les solutions existantes.
•	Une Architecture Technologique Robuste : Le choix des microservices garantit une scalabilité et une fiabilité supérieures, permettant de gérer un grand nombre d'utilisateurs et de pharmacies sans dégradation des performances.
•	Un Modèle de Partenariat Proactif : Une équipe dédiée à l'onboarding et au support des pharmacies pour garantir un réseau dense et fiable dès le lancement.

IV. Proposition de Solution : MediFind

3.1 Vision du projet
MediFind ambitionne de devenir la plateforme de référence et l'écosystème numérique de confiance pour l'accès aux produits de santé en Afrique de l'Ouest, en commençant par un pays pilote. Au-delà de la simple recherche, nous visons à créer un écosystème connectant intelligemment les patients, les pharmacies et les acteurs de la santé.

3.2 Principes de conception
•	Orientation Microservices : Découplage des fonctions métier pour une maintenance, une mise à jour et une scalabilité indépendantes.
•	API-First : Toutes les fonctionnalités sont exposées via des API bien documentées (OpenAPI), permettant de futures intégrations (avec des assureurs, des applications de santé, etc.).
•	Expérience Mobile-First : La conception de l'interface utilisateur est pensée en priorité pour l'application mobile, l'usage principal, puis adaptée pour le web.
•	Sécurité et Confidentialité by Design : La protection des données des utilisateurs et la conformité au RGPD (ou lois locales équivalentes) sont intégrées dès la phase de conception.

3.3 Objectifs fonctionnels et non fonctionnels
•	Fonctionnels :
o	Recherche par nom de médicament avec suggestion automatique.
o	Géolocalisation automatique ou saisie manuelle de la localisation.
o	Affichage des résultats sur une carte et sous forme de liste.
o	Filtrage et tri des résultats par : distance, prix (croissant/décroissant), disponibilité.
o	Fiche détaillée de chaque pharmacie (horaires, contacts, avis utilisateurs* - *phase II).
o	Itinéraire pas-à-pas intégré.
•	Non Fonctionnels :
o	Performance : Temps de réponse de l'API < 200ms pour 95% des requêtes.
Service	Description Fonctionnelle	Base de Données / API Associée	Responsabilités Clés
Service Authentification	Gère le cycle de vie des utilisateurs (inscription, connexion, réinitialisation de mot de passe) et contrôle d'accès (RBAC).	Firebase Authentication	Émission de tokens JWT, gestion des sessions, sécurité des endpoints.
			
Service Catalogue	Cœur métier de l'application. Gère les référentiels des médicaments (nom, DCI, dosage, forme), les stocks et les prix associés à chaque pharmacie.	PostgreSQL (Schéma Catalogue)	Recherche et indexation des médicaments, agrégation des stocks/prix.
Service Pharmacies	Gère les données des officines partenaires : coordonnées, géolocalisation (lat/long), horaires, informations de contact, statut (ouvert/fermé).	PostgreSQL (Schéma Géospatial)	Calcul de proximité, gestion des profils pharmacie.
Service Itinéraire	Service proxy qui interroge l'API Google Maps Directions pour calculer et renvoyer un itinéraire optimisé entre l'utilisateur et une pharmacie.	API Google Maps	Abstraction de l'API externe, mise en cache des trajets fréquents.
Service Prix & Comparaison	Reçoit les données de stock/prix du service Catalogue et implémente la logique de tri et de comparaison des résultats.	Données en mémoire (cache)	Algorithme de classement, application des filtres de prix.
o	Sécurité : Chiffrement des données en transit (TLS 1.3) et au repos, authentification à deux facteurs (2FA) proposée.
o	Scalabilité : Architecture capable de supporter une augmentation de 500% du nombre d'utilisateurs sans refonte.

3.4 Modèle économique et stratégie de partenariat
•	Gratuité pour l'utilisateur final pour assurer une adoption massive.
•	Modèle Freemium pour les pharmacies :
o	Offre de base gratuite : Gestion des stocks pour 50 médicaments, visibilité dans l'application.
o	Offre Premium : Abonnement mensuel pour un nombre illimité de médicaments, statistiques avancées sur les recherches, mise en avant dans les résultats, fonction de réservation en ligne.

V. Architecture et Conception du Système

4.1 Vue d’ensemble de l’architecture
L'architecture repose sur une approche microservices moderne, où chaque service est dédié à un domaine métier précis. Tous les services communiquent via une API Gateway unique qui sert de point d'entrée sécurisé et gère le routage, l'authentification et la limitation du débit (rate limiting).

4.2 Description détaillée des microservices

4.3 Schéma fonctionnel et flux d’information
Flux typique d'une recherche :
1.	L'utilisateur saisit "Doliprane 1000mg".
2.	La requête est routée via l'API Gateway.
3.	Le Gateway valide le token JWT avec le Service Authentification.
4.	Une fois authentifié, la requête est envoyée au Service Catalogue.
5.	Le Service Catalogue interroge la base de données et renvoie la liste des pharmacies ayant le produit.
6.	Le Service Pharmacies enrichit ces résultats avec les données de localisation et de distance.
7.	Le Service Prix applique les filtres et le tri demandés par l'utilisateur.
8.	L'API Gateway agrège la réponse finale et la renvoie au client.
4.4 Sécurité, performance et interopérabilité
•	Sécurité :
o	Authentification : Firebase Auth avec OAuth2 et tokens JWT (JSON Web Tokens) de courte durée.
o	Autorisation : Contrôle d'accès basé sur les rôles (User, Pharmacien, Admin).
o	Chiffrement : HTTPS/TLS obligatoire pour toutes les communications. Chiffrement des données sensibles dans la base (ex: numéros de téléphone).
o	Audit : Journalisation (logging) centralisée de toutes les actions sensibles.
•	Performance :
o	Cache : Mise en œuvre de Redis pour mettre en cache les résultats de recherche fréquents et les données géographiques statiques.
o	Compression : Activation de GZIP sur les réponses JSON de l'API Gateway.
o	Base de données : Indexation avancée sur les champs de recherche (nom de médicament, localisation) et utilisation des extensions PostGIS pour les requêtes géospatiales.
•	Interopérabilité :
o	Tous les microservices exposent des API RESTful avec une documentation OpenAPI (Swagger).
o	Conception des payloads JSON pour faciliter les intégrations futures avec des systèmes tiers (logiciels de gestion de pharmacie, partenaires de livraison).

4.5 Gestion des données et modèle conceptuel
•	SGBD Principal : PostgreSQL, choisi pour sa fiabilité, son support des types de données JSON et ses puissantes extensions géospatiales (PostGIS).
•	Modèle de données clé :
o	Entité Medicament : ID, Nom, DCI, Dosage, Forme galénique.
o	Entité Pharmacie : ID, Nom, Adresse, Coordonnées GPS (Lat/Long), Téléphone, Horaires.
o	Entité Stock : ID_Pharmacie (FK), ID_Medicament (FK), Quantité, Prix, DateMiseÀJour.
o	Entité Utilisateur : ID, Email (hashé), Rôle, Profil (stocké dans Firebase Auth et répliqué en base si besoin).

VI. Technologies Proposées

5.1 Choix technologiques et justifications
Domaine	Technologie	Justification Détaillée
Backend	Spring Boot (Java)	Écosystème mature, excellente prise en charge des microservices, sécurité robuste (Spring Security), vaste communauté et bibliothèques pour l'intégration.
Frontend Web	Angular	Framework complet et structurant, idéal pour des applications d'entreprise riches en fonctionnalités. TypeScript apporte de la rigueur et une meilleure maintenabilité.
Mobile	Flutter	Compilation native pour des performances optimales, "hot reload" pour un développement rapide, code unique pour iOS et Android, UI cohérente et moderne.
Base de Données	PostgreSQL	SGBD relationnel le plus avancé, open-source. Support des requêtes géospatiales (PostGIS), des types JSON et d'une réplication native.
Authentification	Firebase Auth	Service managé, sécurisé et scalable. Prend en charge plusieurs fournisseurs (Google, Facebook), l'authentification par téléphone et la 2FA, réduisant le temps de développement.
Conteneurisation	Docker	Standard de fait pour la création d'images conteneurisées, garantissant la cohérence entre les environnements de développement, test et production.
Orchestration	Kubernetes	(Phase II) Orchestrateur standard pour l'automatisation du déploiement, de la mise à l'échelle et de la gestion des conteneurs, assurant haute disponibilité et résilience.
API Cartes	Google Maps Platform	Solution la plus complète et précise pour les cartes, la géolocalisation et le calcul d'itinéraires. Documentation et support excellents.

5.2 Outils de développement, test et intégration
•	Environnement de Développement Intégré (IDE) : IntelliJ IDEA (backend), VS Code (frontend web & Flutter).
•	Gestion de Version : Git avec hébergement sur GitHub.
•	Tests :
o	Backend : JUnit, Mockito pour les tests unitaires et d'intégration.
o	API : Postman/Newman pour les tests de contrats et les collections d'API.
o	Frontend : Karma/Jasmine (Angular), Flutter Test.
•	Documentation API : Swagger UI/OpenAPI 3.0 générée automatiquement depuis le code.
•	Surveillance : Prometheus pour la collecte de métriques et Grafana pour le dashboarding et les alertes.

5.3 Stratégie de déploiement et configuration
•	Environnements :
o	Développement : Docker Compose sur les machines locales pour un setup rapide et isolé.
o	Staging : Environnement miroir de la production, déployé sur le cloud (AWS/Azure) pour les tests de validation.
o	Production : Cluster de serveurs cloud (ex: AWS EC2 ou Azure VMs) avec load balancer, déploiement initial manuel puis automatisé via CI/CD.
•	Pipeline CI/CD (Intégration Continue / Déploiement Continu) :
1.	Déclenchement : Sur un push sur la branche main ou develop.
2.	Build & Test : GitHub Actions build les images Docker, exécute la suite de tests.
3.	Sécurité : Scan des dépendances (ex: Snyk) et de l'image Docker.
4.	Déploiement Staging : Déploiement automatique sur l'environnement de staging.
5.	Déploiement Production : Déclenchement manuel après validation pour déployer en production (blue-green deployment envisagé en phase II).
5.4 Stratégie de sauvegarde et reprise après sinistre
•	Sauvegardes Automatiques : Sauvegardes quotidiennes et incrémentielles de la base de données PostgreSQL avec rétention de 30 jours.
•	Récupération : Objectif de RTO (Recovery Time Objective) de 4 heures et de RPO (Recovery Point Objective) de 1 heure pour la phase I.
•	Plan de Reprise d'Activité (PRA) : Documentation détaillée pour restaurer l'application complète sur une infrastructure de secours en cas de défaillance majeure.

VII. Calendrier d’Activités et Jalons (Phase I — 12 Mois)

6.1 Étapes de développement détaillées
Période	Jalon Clé	Activités Principales Détailées	Livrables Principaux
Mois 1 – 2	Conception Détaillée & POC	Spécifications techniques détaillées, modélisation des données, mise en place de l'environnement Docker, développement des POC pour les services Auth et Catalogue.	Document de Conception, Repository Git initialisé, POC Auth/Catalogue fonctionnel.
Mois 3 – 5	Développement des Services Cœur	Implémentation complète des services Pharmacies, Itinéraire et Prix. Intégration des API externes (Google Maps). Développement des scripts SQL et des index.	Services backend fonctionnels et testés individuellement, API documentée (Swagger).
Mois 6 – 8	Intégration Frontend & UI/UX	Développement de l'interface utilisateur Web (Angular) et Mobile (Flutter). Intégration avec les API backend. Réalisation des tests d'acceptation utilisateur (UAT).	Application Web et Mobile bêta interne, prêtes pour les tests utilisateurs.
Mois 9 – 10	Tests Intensifs & Validation	Tests de charge (Load Testing) avec JMeter, tests de sécurité (penetration testing), tests d'utilisabilité avec un panel bêta, correction des bugs.	Rapport de tests de performance et de sécurité, liste des bugs résolus, application stable.
Mois 11	Préparation au Lancement	Finalisation de la documentation utilisateur et technique. Formation des pharmaciens partenaires pilotes. Campagne de communication pré-lancement.	Documentation finale, premiers pharmaciens onboardés, page de présentation en ligne.
Mois 12	Lancement du MVP	Déploiement en production. Monitoring actif des performances et des erreurs. Collecte et analyse des retours terrains pour itération.	Application MediFind en ligne et accessible au public.

6.2 Méthodologie de gestion de projet
•	Cadre Agile Scrum : Travail en sprints de 2 semaines avec des objectifs clairs.
•	Rituels : Daily Stand-up, Sprint Planning, Sprint Review & Retrospective.
•	Outil de Gestion : Jira ou Trello pour le suivi des tâches et des bugs.
•	Transparence : Tableaux de bord partagés avec les parties prenantes.

6.3 Indicateurs de performance et livrables
•	Indicateurs Techniques : Temps de réponse API (<200ms), Taux de disponibilité (>99.5%), Taux d'erreur (<0.1%).
•	Indicateurs Métier : Nombre d'utilisateurs actifs mensuels (MAU), nombre de pharmacies partenaires, nombre de recherches effectuées, taux de satisfaction utilisateur (NPS > 50).
•	Livrables Principaux : Code source, documentation technique et utilisateur, application déployée, rapports de test.

6.4 Analyse des risques et plan d'atténuation
Risque Identifié	Impact	Probabilité	Mesure d'Atténuation
Adoption lente par les pharmacies	Élevé	Moyenne	Programme de partenariat proactif, offre de base gratuite, démonstration de la valeur ajoutée.
Données de stock inexactes	Élevé	Moyenne	Interface pharmacien ultra-simple, notifications de rappel de mise à jour, système de "confiance" basé sur l'historique des mises à jour.
Problèmes de performance à l'échelle	Moyen	Faible	Tests de charge rigoureux, architecture scalable dès le départ, monitoring proactif.
Problèmes de sécurité (fuite de données)	Élevé	Faible	Intégration de la sécurité dès la conception, audits de code, formation de l'équipe.

VIII. Conclusion et Prochaines Étapes

7.1 Synthèse globale
MediFind n'est pas simplement une application de plus ; c'est une infrastructure numérique essentielle qui répond à un besoin sociétal concret. Son approche modulaire, centrée sur l'utilisateur et construite sur des technologies robustes, en fait un projet viable, scalable et à fort impact potentiel sur l'efficacité du système de santé.

7.2 Perspectives d’évolution à moyen terme (Phases II & III)
•	Phase II (Mois 13-18) :
o	Fonction de Réservation/Rappel : Permettre à l'utilisateur de "mettre de côté" un médicament.
o	Paiement Mobile Intégré : Intégration avec des solutions de paiement électronique locales (Orange Money, MTN Mobile Money, etc.).
o	Module de Livraison : Partenariat avec des services de livraison pour offrir l'option "à domicile".
•	Phase III (Mois 19-24) :
o	Gestion des Ordonnances : Numérisation et partage sécurisé des ordonnances.
o	Système de Recommandation Intelligent : Suggestions basées sur l'historique et les recherches similaires.
o	Extension aux Parapharmaceutiques : Ajout des produits de bien-être, de puériculture, etc.

7.3 Recommandations finales
1.	Validation Légale : S'assurer de la conformité du projet avec la réglementation nationale sur la vente de médicaments en ligne et la protection des données de santé (CNIL locale).
2.	Partenariat Stratégique : Approcher les ordres nationaux des pharmaciens pour un partenariat officiel, garantissant une crédibilité et une adoption accélérée.
3.	Focus Utilisateur : Maintenir une boucle de feedback continue avec les utilisateurs bêta pour itérer rapidement et améliorer constamment le produit en fonction des retours terrains.
