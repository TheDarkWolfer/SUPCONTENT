# Trello board
Nous avons décidé d'utiliser Trello poru l'organisation ; le panneau est public, et toute demande de droits d'écriture peut être dirigée à Camille, à l'adresse mail [camille.prado@supinfo.com](mailto:camille.prado@supinfo.com)

[Lien Trello](https://trello.com/invite/b/69981ebedbca169f2fc3ce10/ATTI93eda92611a4fe6b4a0170422a15856eA041F1FC/my-trello-board)

# Fonctionnalités à implémenter 
## 1 - Connexion
- [ ] Un utilisateur pourra se connecter à l'application via un compte créé spécifiquement (email/mot de passe) ou en utilisant un compte OAuth2 (Google, Facebook, GitHub, etc.).
- [ ] Un utilisateur ne souhaitant pas créer de compte peut consulter tous les éléments publics de l'application (sans la possibilité d'avoir des interactions) sans créer de compte.

## 2 - Bibliothèque personnelle (Collections)
- [ ] Les utilisateurs peuvent organiser les œuvres dans leur bibliothèque via des statuts prédéfinis.
- [ ] Listes par défaut : "À voir/lire/jouer/etc.", "En cours", "Terminé", "Abandonné".
- [ ] Listes personnalisées : L'utilisateur peut créer des listes thématiques (ex: "Mes films d'horreur préférés", "Lectures d'été ## ") et les rendre publiques ou privées.
- [ ] Un tableau de bord permet de visualiser les statistiques de sa collection (nombre d'œuvres terminées, temps passé, etc.).

## 3 - Fiches média & critiques
- [ ] Chaque œuvre dispose d'une page dédiée générée à partir des données de l'API externe combinées aux données de SUPCONTENT.
- [ ] Informations générales : Résumé, date de sortie, auteur/réalisateur (données API tierce).
- [ ] Espace communautaire : Moyenne des notes des utilisateurs de SUPCONTENT, liste des critiques, discussions associées.
- [ ] Action utilisateur : Possibilité de noter (étoiles), de rédiger une critique détaillée (texte avec formatage) et d'ajouter l'œuvre à une liste.

## 4 - Interaction sociale & Fil d'actualité
- [ ] Un système de "Follow" (abonnement) permet de suivre d'autres utilisateurs.
- [ ] Fil d'actualité : Agrégation chronologique des activités des amis (Notes attribuées, critiques publiées, entrées dans une collection).
- [ ] Interactions : Possibilité de "Liker" une critique ou de la commenter.
- [ ] Messagerie privée : Système de chat simple entre deux utilisateurs qui se suivent mutuellement.

## 5 - Modération et rôles
- [ ] Administrateurs : Peuvent modérer les critiques signalées (suppression de contenu inapproprié), bannir des utilisateurs, et mettre en avant certaines critiques ("Coups de cœur").
- [ ] Utilisateurs : Peuvent signaler un contenu (spoilers non marqués, insultes).

## 6 - Notifications
- [ ] Notifications en temps réel :
    - [ ] Nouveau "J'aime" ou commentaire sur une critique.
    - [ ] Nouvel abonné.
    - [ ] Recommandation automatique basée sur les goûts (ex: "Un nouveau livre de votre auteur favori est sorti").
    - [ ] Options de personnalisation (Push ou Email).

## 7 - Intégration API tierce
- [ ] L'application ne doit pas stocker la totalité des données des œuvres en base de données, mais doit agir comme un cache ou un enrichisseur.
- [ ] Recherche : La barre de recherche interroge l'API tierce en temps réel.
- [ ] Synchronisation : Importation intelligente des données nécessaires à l'affichage (Images, Titres) pour limiter les appels API redondants.

## 8 - Recherche avancée
- [ ] Recherche unifiée permettant de trouver :
    - [ ] Des œuvres (via l'API externe) avec filtres (genre, année, auteur).
    - [ ] Des utilisateurs de la plateforme.
    - [ ] Des listes publiques créées par la communauté.

## 9 - Paramètres utilisateurs
- [ ] Gestion de profil : Avatar, biographie, lien vers site web.
- [ ] Préférences : Thème (Clair/Sombre), langue de l'interface.
- [ ] Exportation des données personnelles (Liste des œuvres notées au format CSV/JSON - conformité RGPD).

## 10 - Conteneurisation
- [ ] Docker compose pour :
    - [ ] Client web
    - [ ] Serveur
    - [ ] Base de données

# Rôles clef :
## Camille :
- Gestion du dépôt Github & Trello
- Tests de sécurité
- Assistance dev
## Dimitri :
- Architecture frontend
- Dev
## Rafael :
- Architecture backend
- Dev
## Jean-Loic :
- Dev polyvalent
