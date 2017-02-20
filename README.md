# Rapport de projet Android
Réalisation d'une application BDE destinée aux étudiants.  
Cette application comporte les deux foncitonnalités principales suivantes :
- Permettre aux étudiants de s'informer sur les prochains évènements du BDE, et les ajouter à leur agenda
- Permettre aux étudiants de trouver et ouvrir des annales pour leur révision. Nous utiliserons la base de données d'annales collaborative déjà existante sur http://bde.esiee.fr/annales

1. [Description fonctionnelle du projet](#description-fonctionnelle-du-projet)
  - Choix des fonctionnalités
  - Le design et l'UI
  - Animations
2. [Description technique du projet](#description-technique-du-projet)
  - Le framework React Native
  - Challenges Rencontrés
  - Modules utilisés
  - Le Backend

## Description fonctionnelle du projet

### Choix des fonctionnalités

Nous avons choisi d'implémenter en priorité les deux fonctionalités les plus utilisées sur notre site internet, et les plus chères aux étudiants : La recherche d'annales et la consultation des évènements du BDE.
La consultation des évènements du BDE doit être rapide, et afin que l'utilisateur n'aie pas à constamment faire appel à l'application du BDE, nous avons souhaité lui donner la possibilité d'ajouter l'évènement à l'agenda de son téléphone.
Quant à la recherche d'annales, nous avons mis au centre de cet fonctionnalité un champ de recherche fonctionnant avec toutes les métadonnées du document : Année scolaire, Niveau (E1,E2...), Professeur, Matière, Code de l'unité, etc..

Les recherches "2016 Android", "E4 SI-4201", ou "Raynal Cours E4" peuvent donc toutes fonctionner.

### Le design et L'UI

### Animations

## Description technique du projet

