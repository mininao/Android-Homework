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

### React Native

React Native est une bibliothèque javascript et un ensemble d'outils permettant de développer tout ou partie d'une application mobile en javascript. Elle a été créée par facebook sur la base de React, une bibliothèque similaire destinée au navigateur.   
Elle permet notamment de partager une grande quantitée de code entre les versions iOS et Android d'une application, mais reste basée sur des composants d'UI natifs, atteignant ainsi de très bonnes performances (contrairement aux outils similaires jusqu'ici basés sur des webviews).  
Malgré sa relative nouveautée, React Native est utilisé dans de nombreuses Applications : Facebook, Instagram, Airbnb, Soundcloud l'utilisent en production.
J'ai donc choisi de l'utiliser, afin qu'une fois la version Android terminée, je puisse publier une version iOS au plus vite.

### Challenges rencontrés


### Modules utilisés
La communauté react native est particulièrement active, et nous permet de bénéficier ainsi de nombreux modules open-source. On note qu'il est souvent nécessaire d'utiliser d'avantage de modules avec react-native qu'en développement natif, les créateurs de react native ayant la volonté de garder leur framework assez léger. Nous avons utilisé les suivants :
- [react-native-google-signin](https://www.npmjs.com/package/react-native-google-signin)
  Permet d'authentifier l'utilisateur via l'authentification google. Ce module s'est révélé toutefois difficile à intégrer et nous avons dû downgrader notre version de react-native pour qu'il soit fonctionnel.
- [react-native-linear-gradient](https://www.npmjs.com/package/react-native-linear-gradient)
  Ce module fort pratique permet d'afficher des dégradés, par ailleurs non gérés par react native
- [react-native-router-flux](https://www.npmjs.com/package/react-native-router-flux)
  Ce module permet de créer un "routeur", qui à l'instar du système d'url sur internet, permet de gérer différentes "scènes" au sein de l'application
- [react-native-scrollable-tab-view](https://www.npmjs.com/package/react-native-scrollable-tab-view)
  Ce module permet d'implémenter le mécanisme de scroll horizontal entre les différents onglets visibles au bas de l'application.
- [react-native-vector-icons](https://www.npmjs.com/package/react-native-vector-icons)
  Ce module gère l'importation de fonts d'icônes, et leur utilisation via un élément `<Icon>`

### Le backend
J'ai réalisé le backend avec le framework php symfony et avec l'aide de mon coéquipier technique au BDE, Naji Astier.
