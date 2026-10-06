# Badgeuse de chantier — CHOK'BÉTON

Application de pointage pour chantier, utilisable depuis un téléphone **sans compte et sans réseau**.

Un téléphone posté à l'entrée du chantier sert de badgeuse : chaque compagnon appuie sur son nom,
saisit son code à 4 chiffres et pointe son arrivée puis son départ.

## Fonctions

- **Retard calculé** par rapport à l'heure d'arrivée prévue, avec une tolérance réglable.
- **Motif du retard** demandé au-delà de la tolérance (train, bus, covoiturage, circulation…),
  utile pour une équipe non véhiculée.
- **Position GPS** : enregistrement de la position du chantier, distance affichée à chaque pointage,
  et option de refus du pointage hors d'un rayon donné.
- **Tableau du jour** : à l'heure / en retard / pas encore pointé, avec le cumul des retards.
- **Historique 30 jours** par compagnon et **export CSV** pour la paie.
- **Sauvegarde / restauration** par fichier `.json`.

## Installation sur le téléphone

Ouvrir l'adresse du site, puis **« Ajouter à l'écran d'accueil »**.
L'application s'ouvre ensuite en plein écran, avec son icône, et fonctionne hors réseau.

## Premiers réglages

1. Onglet **Réglages**, code par défaut `1234` — à changer immédiatement.
2. Ajouter les compagnons avec leur code à 4 chiffres (le premier ajout retire l'équipe d'exemple).
3. Depuis le chantier : **« Enregistrer ma position comme chantier »**.

## Où sont les données

Dans le téléphone qui badge, et nulle part ailleurs : aucun compte, aucun serveur, aucune donnée
envoyée. Exporter une sauvegarde régulièrement depuis l'onglet Réglages.

## Fichiers

| Fichier | Rôle |
|---|---|
| `index.html` | L'application entière (HTML, CSS et JavaScript) |
| `sw.js` | Cache hors ligne |
| `manifest.webmanifest` | Installation sur l'écran d'accueil |
| `icone.svg` | Icône |
