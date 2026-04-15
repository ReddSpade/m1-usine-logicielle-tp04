# Compte Rendu

## Partie 0 — État des lieux

## Partie 1 — Scan de dépendances avec pip-audit

### Question 1

#### Qu'est-ce qu'une CVE ? Expliquez le score CVSS et donnez un exemple de CVE avec son impact. <!-- rumdl-disable-line MD013 -->

Une CVE ou Common Vulnerability and Exposure est vulnérabilité dans un logiciel
ou matériel qui peut être exploitée pour compromettre la sécurité d'un système.

Le score CVSS ou Common Vulnerability Scoring System quant à lui est un système
de notation entre 1 et 10 qui évalue la sévérité d'une CVE.

Si on regarde le [top 10 des CVE de 2020](https://www.cert.ssi.gouv.fr/actualite/CERTFR-2021-ACT-008/), on peut prendre en exemple la CVE
CVE-2020-0688, venant de Microsoft sur les services Exchange.

Avec cette vulnérabilité, on peut exécuter du code à distance si on est un
utilisateur authentifié.

### Question 2

#### Pourquoi est-il important de scanner les dépendances et pas seulement votre propre code ? <!-- rumdl-disable-line MD013 -->

L'importance de scan de dépendances est assez évidente, cela évite d'implémenter
dans son code des packages qui seraient compromis, ou de faire tourner du code compromis.

## Partie 2 — Dependabot : mises à jour automatiques

### Question 3

#### Quel est l'avantage de Dependabot par rapport à un scan manuel avec pip-audit ? Pourquoi configure-t-on aussi l'écosystème github-actions ? <!-- rumdl-disable-line MD013 -->

## Partie 3 — Gestion des secrets avec GitHub Secrets

### Question 4

#### Pourquoi ne doit-on jamais mettre un secret directement dans le code source ? Citez 3 endroits où stocker des secrets de manière sécurisée. <!-- rumdl-disable-line MD013 -->

## Partie 4 — Détection de secrets avec GitLeaks

### Question 5

#### Un développeur a accidentellement commité une clé API GCP dans le code, puis l'a supprimée dans un commit suivant. Le secret est-il en sécurité ? Que faut-il faire ? <!-- rumdl-disable-line MD013 -->

### Question 6

#### Pourquoi GitLeaks est-il placé au tout début du pipeline, avant même le linting ? <!-- rumdl-disable-line MD013 -->

## Partie 5 — Pipeline de sécurité complet

### Question 7

#### Citez 3 risques de l'OWASP Top 10 et expliquez comment votre pipeline CI les adresse (ou pas). <!-- rumdl-disable-line MD013 -->

### Question 8

#### Décrivez l'ordre complet de votre pipeline final. Pour chaque étape, indiquez quel type de problème elle détecte. <!-- rumdl-disable-line MD013 -->

### Question 9

#### Comparez les approches Shift Left et audit de sécurité traditionnel. Quels sont les avantages du Shift Left ? <!-- rumdl-disable-line MD013 -->

### Question 10

#### Votre pipeline contient maintenant de nombreuses étapes. Si le temps d'exécution devenait trop long, comment pourriez-vous l'optimiser ? <!-- rumdl-disable-line MD013 -->

## Partie 6 — Recherche autonome

### Question 11

#### Décrivez la CVE que vous avez trouvée : son identifiant, le package affecté, le score CVSS, l'impact, et la version corrigée. Expliquez comment pip-audit ou Dependabot aurait pu prévenir ce problème. Indiquez le lien vers la page de la CVE. <!-- rumdl-disable-line MD013 -->
