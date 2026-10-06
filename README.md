# Idris El Hannach

Étudiant en **M1 Sciences des données pour l'ingénieur·e (SCDI)**, Sorbonne Université & ISUP.
Je recherche un **stage de Data Scientist de 2 à 3 mois, de juin à août 2027**.

📫 idriselhannach@gmail.com

---

## Sirocco

Application mobile (iOS, Android) et web qui réunit les Français à l'étranger et les
étudiants d'une même ville ou école autour d'événements. En production depuis l'été 2026 :
**près de 50 membres, 6 communautés** (Marrakech, Paris, Londres, Barcelone, Berlin, ESSEC),
**5 langues** dont l'arabe, lu de droite à gauche.

> Le code est privé : démonstration et visite du code sur demande.

### Ce qui touche aux données

- **Système de recommandation.** Le fil et les événements sont classés pour chaque membre :
  un score de fraîcheur à décroissance exponentielle (demi-vie de 30 heures), pondéré par
  l'affinité (liens sociaux, auteurs aimés, mots-clés des contenus enregistrés ou lus
  jusqu'au bout, engagement). Une place sur quatre revient à l'exploration, pour ne pas
  enfermer chacun dans ce qu'il connaît, et un même auteur n'occupe jamais trois places de
  suite. Le classement ne s'active qu'au-delà de 20 publications en 48 heures, et se calcule
  sur le téléphone : aucune donnée de lecture ne quitte l'appareil.
- **Données géospatiales.** Maquette 3D du campus de l'ESSEC construite à partir
  d'OpenStreetMap ; géoréférencement de 429 salles issues des plans d'étage et recalage des
  1 780 prises de vue d'une visite virtuelle sur les bâtiments. Les points tombés hors des
  murs sont corrigés automatiquement (point dans un polygone, projection sur le mur le plus
  proche). Chaque communauté a son territoire : les adresses proposées et la carte n'en
  sortent pas.
- **Moteur de points résistant à la fraude.** Les points et trophées sont calculés côté
  serveur, uniquement à partir de faits vérifiés (présence validée par l'organisateur,
  rencontres) : clés d'idempotence, plafonds quotidiens, tests contre un émulateur de base
  de données.
- **Données personnelles.** Base NoSQL dont les règles d'accès sont la seule protection,
  durées de conservation et purge automatique, politique de confidentialité en cinq langues
  (RGPD).

### Technologies

TypeScript · React · Node.js · Firebase (Realtime Database, Cloud Functions, Storage) ·
Capacitor (iOS, Android) · MapLibre et OpenStreetMap · three.js · Vitest · Git

---

## Mémoire de licence : méthodes inverses et assimilation de données

UVSQ, janvier à mai 2026, en équipe de trois, encadré par Maëlle Nodet.
Comment combiner au mieux des observations et une information *a priori* sur l'état d'un
système, en tenant compte de l'incertitude de chacune, avec une application à la
météorologie :

- construction de l'estimateur **BLUE** (*Best Linear Unbiased Estimator*), en scalaire
  puis en vectoriel, à partir des matrices de covariance d'erreur ;
- outils d'optimisation : gradient, multiplicateurs de Lagrange, méthodes de descente ;
- **expérience jumelle** sur des données météorologiques réelles, en Python (NumPy, pandas,
  SciPy, Matplotlib) dans un notebook Jupyter ; rapport rédigé en LaTeX.

---

## Compétences

**Programmation** : Python (NumPy, pandas, SciPy, Matplotlib, Jupyter), SQL, TypeScript / JavaScript, LaTeX
**Mathématiques** : probabilités, statistique, apprentissage statistique, optimisation, séries temporelles
**Langues** : français, anglais (B2), espagnol (B1)
