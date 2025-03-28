# 🧠 Autopilot Car Simulator (Browser Edition)

Ce projet est une simulation simple d’un système d’autopilot embarqué directement dans le navigateur à l’aide de JavaScript et Canvas.  
Il met en œuvre un **Lane Keeping Assist (LKA)** basique basé sur une détection de trajectoire simulée, avec un rendu visuel animé en top-down.

---

## 🚗 Fonctionnalités

- ✅ **Vue top-down** d’une voiture autonome sur une route courbée
- ✅ **Trajectoire personnalisée** (circuit) dessinée avec Canvas
- ✅ **Voiture en mouvement automatique**, suivant la route grâce à un algorithme de correction d’erreur
- ✅ **Système de capteur simulé** (rayon jaune) pour détecter la distance à la trajectoire
- ✅ **Arbres générés dynamiquement** pour décorer l’environnement

---

## 🧪 Comment ça marche

- Un **capteur virtuel** est placé devant la voiture pour détecter la position par rapport à la route.
- Un algorithme proportionnel (`P-controller`) corrige l’orientation de la voiture selon l’erreur latérale mesurée.
- Le véhicule avance automatiquement tout en corrigeant sa direction pour rester centré sur la route.

---

## 📁 Fichiers

- `index.html` : contient tout le code JavaScript et HTML nécessaire à la simulation.
- Aucun framework requis — tout fonctionne directement dans le navigateur.

---

## ✅ Lancer la démo

1. Ouvrez simplement `index.html` dans un navigateur moderne (Chrome, Firefox…).
2. La simulation démarre automatiquement.

---

## 🔧 Paramètres clés

- `Kp` : constante de proportion pour corriger l’angle de la voiture (tuning possible)
- `path[]` : liste des points représentant le circuit
- `car.speed` : vitesse de la voiture simulée

---

## 📊 Présentation

Une présentation est fournie pour expliquer :

- L’architecture générale du projet
- Les algorithmes utilisés (capteur, détection d’erreur, correction)
- Les choix de design et limitations

> Le lien vers la présentation (PDF, Canva ou PowerPoint) sera ajouté ici.

---

## 👨‍💻 Auteurs

Projet réalisé par :

- **[Ton Prénom Nom]**
- **Clément Dreiski**

---

## 💡 Améliorations possibles

- Ajout d’un **véhicule précédent** pour simuler un système d’**Adaptive Cruise Control (ACC)**
- Utilisation d’un vrai algorithme PID (avec dérivée et intégrale)
- Interface utilisateur pour changer les paramètres à la volée
- Détection dynamique de la trajectoire via caméra simulée

---

## 📝 Ressources & Inspirations

- [commaai/openpilot](https://github.com/commaai/openpilot) – Pour les principes de pilotage autonome
- Concepts de base en robotique mobile (capteurs, suivi de trajectoire)

---

> 🔔 **IMPORTANT** : Un seul membre du groupe doit soumettre le projet avec les noms des deux membres.
