
---

## Accès et outils

- [ ] Accès au **dépôt Git** (GitHub / GitLab / Bitbucket) — demander une invitation
- [ ] Accès au **gestionnaire de projet** (Jira, Trello, Linear, Odoo Projet…)
- [ ] Accès à la **messagerie d'équipe** (Slack, Teams, Discord…)
- [ ] Accès à la **documentation interne** (Notion, Confluence, wiki, Obsidian partagé…)
- [ ] Accès aux **environnements** : staging, prod, Odoo.sh (si applicable)
- [ ] VPN ou accès réseau si infra on-premise
- [ ] Récupérer les **identifiants PgAdmin / base de données** de dev

---

##  Comprendre l'environnement technique

- [ ] Quelle **version d'Odoo** est utilisée ? (CE, Enterprise, Odoo.sh ?)
- [ ] Comment est structuré le **docker-compose** ? (services, volumes, réseaux)
- [ ] Où sont les **modules custom** ? (dépôt dédié, mono-repo, sous-dossier ?)
- [ ] Y a-t-il un fichier **`odoo.conf`** partagé ou chacun le configure localement ?
- [ ] Quelle version de **PostgreSQL** est utilisée ?
- [ ] Y a-t-il des **modules OCA** installés ? Lesquels ?
- [ ] Existe-t-il un **script de setup** pour monter l'env de dev ? (`Makefile`, `README`, script bash…)

---

## Comprendre le workflow de l'équipe

- [ ] Quel est le **modèle de branches** ? (`main`/`dev`/`staging` ? GitFlow ? Trunk-based ?)
- [ ] Y a-t-il des **conventions de commit** ? (Conventional Commits, préfixes custom…)
- [ ] Quel est le **process de code review** ? (PR obligatoire ? Nombre d'approbations ?)
- [ ] Y a-t-il de la **CI/CD** ? (tests auto, lint, déploiement automatique ?)
- [ ] Comment se font les **déploiements** en staging et en prod ?
- [ ] Y a-t-il des **tests unitaires** ou fonctionnels sur les modules custom ?

---

## Première semaine

- [ ] Cloner le(s) dépôt(s)
- [ ] Lancer le `docker-compose up` et vérifier que tout tourne
- [ ] Restaurer une **base de dev/staging** en local
- [ ] Installer les **modules custom** et vérifier qu'ils chargent
- [ ] Configurer son **éditeur** (VS Code, PyCharm…) avec les bons linters/formatters de l'équipe
- [ ] Tester un cycle complet : modifier un module → relancer → vérifier le changement
- [ ] Quel est le **secteur d'activité** des clients ? (e-commerce, industrie, services…)
- [ ] Quels **modules fonctionnels** Odoo sont les plus utilisés ? (Ventes, Stock, Compta, POS, MRP…)
- [ ] Y a-t-il un **client principal** ou plusieurs projets en parallèle ?
- [ ] Qui est le **référent technique** pour les questions Odoo ?
- [ ] Existe-t-il une **base de connaissances** sur les choix techniques passés ?

---

## Questions à ne pas oublier

- "Comment on gère les **mises à jour de modules** en prod ?"
- "Il y a un **environnement de recette** séparé pour les clients ?"
- "On utilise **OpenUpgrade** ou la migration se fait via Odoo.sh / Odoo SA ?"
- "Qui a accès au **serveur de prod** et comment ?"
- "Il y a des **sauvegardes automatiques** ? À quelle fréquence ?"