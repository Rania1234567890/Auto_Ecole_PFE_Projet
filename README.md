#  Auto-École — Plateforme de Gestion

Application web complète pour la gestion d'une auto-école.

![Capture d'écran](screenshots/hero.png)

##  Fonctionnalités

-  Gestion des candidats et moniteurs
-  Suivi de progression (HighWay Code / Parking / Driving)
-  Planning hebdomadaire automatisé
-  Gestion de flotte de véhicules
-  Leçons théoriques + tests pratiques
-  Demandes de changement de session
-  3 rôles : Admin / Monitor / Candidate

## Tech Stack

- **Backend** : PHP 8 (procédural + POO)
- **Base de données** : MySQL (InnoDB)
- **Frontend** : HTML5, CSS3 (glassmorphism), JavaScript
- **Charts** : Chart.js
- **Hébergement** : InfinityFree

## Sécurité

- Mots de passe bcrypt + pepper
- CSRF sur tous les formulaires
- Requêtes préparées (anti-SQL injection)
- Échappement XSS (`e()`)
- Sessions sécurisées (HttpOnly, SameSite)
- Rate limiting login (5 tentatives / 15 min)
- Upload sécurisé (MIME + taille + nom aléatoire)
- Migration automatique SHA256 → bcrypt

## Installation

1. Cloner le repo :
   ```bash
   git clone https://github.com/ton-user/auto-ecole.git
