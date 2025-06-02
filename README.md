# AMPTranslations : Fichiers de Localisation Multi-Langues pour AMP

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
![Statut de Traduction](https://img.shields.io/badge/statut-active-blue)
Ce dépôt fournit des fichiers de traduction (`.json`) pour divers composants et fonctionnalités **AMP (Accelerated Mobile Pages)** dans plusieurs langues, notamment le **français (fr.json)**, l'**anglais (en.json)**, l'**allemand (de.json)**, l'**espagnol (es.json)** et le **polonais (pl.json)**.

## Pourquoi ce Projet ?

L'objectif est de faciliter l'intégration de traductions dans vos projets AMP, permettant ainsi d'offrir une expérience utilisateur localisée pour une audience internationale. Bien qu'AMP supporte l'internationalisation, obtenir des fichiers de traduction complets et à jour pour toutes les fonctionnalités peut être un défi. Ce dépôt centralise et maintient ces fichiers pour vous.

## Comment Utiliser ces Traductions

Pour intégrer ces traductions dans votre page AMP :

1.  **Téléchargez le fichier de langue souhaité :**
    Sélectionnez et téléchargez le fichier `.json` de la langue dont vous avez besoin directement depuis la racine de ce dépôt (par exemple, `fr.json` pour le français).

2.  **Incluez les traductions dans votre code AMP HTML :**
    Vous pouvez copier le contenu du fichier `.json` et l'intégrer directement dans votre page AMP en utilisant une balise `<script type="application/json">` avec un `id` unique. Ensuite, référencez cet `id` via l'attribut `i18n` sur les éléments AMP qui supportent l'internationalisation.

    **Exemple pour un composant AMP (adapter selon le composant réel) :**

    ```html
    <!doctype html>
    <html ⚡ lang="fr">
    <head>
      <meta charset="utf-8">
      <link rel="canonical" href="[https://example.com/amp-page.html](https://example.com/amp-page.html)">
      <meta name="viewport" content="width=device-width,minimum-scale=1,initial-scale=1">
      <style amp-boilerplate>body{-webkit-animation:-amp-start 8s steps(1,end) 0s 1 normal both;-moz-animation:-amp-start 8s steps(1,end) 0s 1 normal both;-ms-animation:-amp-start 8s steps(1,end) 0s 1 normal both;animation:-amp-start 8s steps(1,end) 0s 1 normal both}@-webkit-keyframes -amp-start{from{visibility:hidden}to{visibility:visible}}@-moz-keyframes -amp-start{from{visibility:hidden}to{visibility:visible}}@-ms-keyframes -amp-start{from{visibility:hidden}to{visibility:visible}}@-o-keyframes -amp-start{from{visibility:hidden}to{visibility:visible}}@keyframes -amp-start{from{visibility:hidden}to{visibility:visible}}</style><noscript><style amp-boilerplate>body{-webkit-animation:none;-moz-animation:none;-ms-animation:none;animation:none}</style></noscript>
      <script async src="[https://cdn.ampproject.org/v0.js](https://cdn.ampproject.org/v0.js)"></script>
      <script async custom-element="amp-carousel" src="[https://cdn.ampproject.org/v0/amp-carousel-0.1.js](https://cdn.ampproject.org/v0/amp-carousel-0.1.js)"></script>
      </head>
    <body>
      <script id="my-fr-strings" type="application/json">
        {
          "AMP_COMP_STRING_1": "Texte traduit 1",
          "AMP_COMP_STRING_2": "Texte traduit 2",
          "NEXT_BUTTON_LABEL": "Suivant",
          "PREVIOUS_BUTTON_LABEL": "Précédent"
        }
      </script>

      <amp-carousel width="400" height="300" layout="responsive" type="slides" controls i18n="my-fr-strings">
        <img src="image1.jpg" alt="Image 1">
        <img src="image2.jpg" alt="Image 2">
      </amp-carousel>

      <div i18n="my-fr-strings" data-i18n-content="AMP_COMP_STRING_1"></div>
      </body>
    </html>
    ```
    **Note :** L'ID du script (`my-fr-strings` dans cet exemple) est arbitraire mais doit correspondre à la valeur de l'attribut `i18n` sur l'élément AMP. Assurez-vous que les clés JSON dans votre fichier (`AMP_COMP_STRING_1`, `NEXT_BUTTON_LABEL`, etc.) correspondent aux chaînes que le composant AMP attend.

3.  **Alternative : Référencement Direct (Si votre serveur le permet)**
    Si votre environnement de serveur web permet un accès direct aux fichiers, vous pourriez potentiellement les placer dans un dossier comme `/Locale/` et les charger dynamiquement, mais l'approche `<script type="application/json">` est la méthode standard et la plus fiable pour AMP.

## Composants et Langues Disponibles

Ce dépôt contient des fichiers de traduction pour les langues suivantes :

* **Français** (`fr.json`)
* **Anglais** (`en.json`)
* **Allemand** (`de.json`)
* **Espagnol** (`es.json`)
* **Polonais** (`pl.json`)

Chaque fichier contient des traductions pour diverses chaînes de caractères utilisées par les composants et le runtime AMP. Examinez les fichiers `.json` pour voir les clés de traduction spécifiques et leur contenu.

## Comment Contribuer

Nous accueillons avec grand plaisir toutes les contributions pour améliorer et étendre ces traductions ! Votre aide est précieuse, que ce soit pour corriger une erreur, suggérer une meilleure traduction, ou ajouter des traductions pour de nouvelles clés ou composants AMP.

1.  **Forkez** ce dépôt.
2.  **Clonez** votre fork localement :
    ```bash
    git clone [https://github.com/votre-utilisateur/AMPTranslations.git](https://github.com/votre-utilisateur/AMPTranslations.git)
    ```
3.  **Créez une nouvelle branche** pour vos modifications :
    ```bash
    git checkout -b feature/amelioration-fr-json
    ```
4.  **Effectuez vos modifications** directement dans les fichiers `.json` exist
