# AMPTranslations : Fichiers de Localisation Multi-Langues pour AMP

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
![Statut de Traduction](https://img.shields.io/badge/statut-active-blue)
Ce dépôt fournit des fichiers de traduction (`.json`) pour divers composants et fonctionnalités **AMP (Accelerated Mobile Pages)** dans plusieurs langues, notamment le **français (fr.json)**, l'**anglais (en.json)**, l'**allemand (de.json)**, l'**espagnol (es.json)** et le **polonais (pl.json)**.

## Comment Utiliser ces Traductions

Pour intégrer ces traductions dans votre page AMP :

1.  **Téléchargez le fichier de langue souhaité :**
    Sélectionnez et téléchargez le fichier `.json` de la langue dont vous avez besoin directement depuis la racine de ce dépôt (par exemple, `fr.json` pour le français).

2.  **Placez les fichiers de traduction dans le répertoire Locale :**
    Copiez les fichiers `.json` téléchargés dans le répertoire `Locale` de votre environnement AMP, par exemple :
    `home\amp\.ampdata\instances\ADS01\WebRoot\Locale\`

3.  **Incluez les traductions dans votre code AMP HTML :**
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
4.  **Effectuez vos modifications** directement dans les fichiers `.json` existants (par exemple, `fr.json`). Assurez-vous de respecter le format JSON valide.
5.  **Commitez vos changements** avec un message clair :
    ```bash
    git commit -m "fix: Correction d'une faute dans fr.json"
    # ou
    git commit -m "feat: Ajout de nouvelles clés pour amp-comp dans en.json"
    ```
6.  **Pushez** votre branche vers votre fork sur GitHub :
    ```bash
    git push origin feature/amelioration-fr-json
    ```
7.  **Ouvrez une Pull Request (PR)** vers la branche `main` de ce dépôt. Décrivez vos modifications et les raisons de celles-ci.

## Source Originale / Original Source

Ce dépôt est un fork et contient des traductions basées sur le travail original de :
**[CubeCoders/AMPTranslations](https://github.com/CubeCoders/AMPTranslations)**

Nous maintenons et améliorons ces traductions pour la communauté francophone (et autres langues) et nous efforçons de rester à jour avec les changements de la source originale.

## Licence

Ce projet est sous licence **MIT**. Voir le fichier [LICENSE](LICENSE) pour plus de détails.

## Remerciements

Un grand merci à tous les contributeurs et à la communauté AMP pour leur travail continu.

---

<br>
<br>

# AMPTranslations: Multi-Language Localization Files for AMP

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
![Translation Status](https://img.shields.io/badge/status-active-blue)
This repository provides translation files (`.json`) for various **AMP (Accelerated Mobile Pages)** components and features in multiple languages, including **French (fr.json)**, **English (en.json)**, **German (de.json)**, **Spanish (es.json)**, and **Polish (pl.json)**.

## How to Use These Translations

To integrate these translations into your AMP page:

1.  **Download the desired language file:**
    Select and download the `.json` file for the language you need directly from the root of this repository (e.g., `en.json` for English).

2.  **Place the translation files in the Locale directory:**
     Copy the downloaded `.json` files into the `Locale` directory of your AMP environment, for example:
     `home\amp\.ampdata\instances\ADS01\WebRoot\Locale\`

3.  **Include the translations in your AMP HTML code:**
    You can copy the content of the `.json` file and embed it directly into your AMP page using a `<script type="application/json">` tag with a unique `id`. Then, reference this `id` via the `i18n` attribute on AMP elements that support internationalization.

    **Example for an AMP component (adapt according to the actual component):**

    ```html
    <!doctype html>
    <html ⚡ lang="en">
    <head>
      <meta charset="utf-8">
      <link rel="canonical" href="[https://example.com/amp-page.html](https://example.com/amp-page.html)">
      <meta name="viewport" content="width=device-width,minimum-scale=1,initial-scale=1">
      <style amp-boilerplate>body{-webkit-animation:-amp-start 8s steps(1,end) 0s 1 normal both;-moz-animation:-amp-start 8s steps(1,end) 0s 1 normal both;-ms-animation:-amp-start 8s steps(1,end) 0s 1 normal both;animation:-amp-start 8s steps(1,end) 0s 1 normal both}@-webkit-keyframes -amp-start{from{visibility:hidden}to{visibility:visible}}@-moz-keyframes -amp-start{from{visibility:hidden}to{visibility:visible}}@-ms-keyframes -amp-start{from{visibility:hidden}to{visibility:visible}}@-o-keyframes -amp-start{from{visibility:hidden}to{visibility:visible}}@keyframes -amp-start{from{visibility:hidden}to{visibility:visible}}</style><noscript><style amp-boilerplate>body{-webkit-animation:none;-moz-animation:none;-ms-animation:none;animation:none}</style></noscript>
      <script async src="[https://cdn.ampproject.org/v0.js](https://cdn.ampproject.org/v0.js)"></script>
      <script async custom-element="amp-carousel" src="[https://cdn.ampproject.org/v0/amp-carousel-0.1.js](https://cdn.ampproject.org/v0/amp-carousel-0.1.js)"></script>
      </head>
    <body>
      <script id="my-en-strings" type="application/json">
        {
          "AMP_COMP_STRING_1": "Translated text 1",
          "AMP_COMP_STRING_2": "Translated text 2",
          "NEXT_BUTTON_LABEL": "Next",
          "PREVIOUS_BUTTON_LABEL": "Previous"
        }
      </script>

      <amp-carousel width="400" height="300" layout="responsive" type="slides" controls i18n="my-en-strings">
        <img src="image1.jpg" alt="Image 1">
        <img src="image2.jpg" alt="Image 2">
      </amp-carousel>

      <div i18n="my-en-strings" data-i18n-content="AMP_COMP_STRING_1"></div>
      </body>
    </html>
    ```
    **Note:** The script ID (`my-en-strings` in this example) is arbitrary but must match the value of the `i18n` attribute on the AMP element. Ensure that the JSON keys in your file (`AMP_COMP_STRING_1`, `NEXT_BUTTON_LABEL`, etc.) match the strings the AMP component expects.

## Available Components and Languages

This repository contains translation files for the following languages:

* **French** (`fr.json`)
* **English** (`en.json`)
* **German** (`de.json`)
* **Spanish** (`es.json`)
* **Polish** (`pl.json`)

Each file contains translations for various strings used by AMP components and the AMP runtime. Examine the `.json` files to see the specific translation keys and their content.

## How to Contribute

We warmly welcome all contributions to improve and expand these translations! Your help is valuable, whether to correct an error, suggest a better translation, or add translations for new AMP keys or components.

1.  **Fork** this repository.
2.  **Clone** your fork locally:
    ```bash
    git clone [https://github.com/your-username/AMPTranslations.git](https://github.com/your-username/AMPTranslations.git)
    ```
3.  **Create a new branch** for your changes:
    ```bash
    git checkout -b feature/en-json-improvement
    ```
4.  **Make your changes** directly in the existing `.json` files (e.g., `en.json`). Ensure the JSON format is valid.
5.  **Commit your changes** with a clear message:
    ```bash
    git commit -m "fix: Corrected a typo in en.json"
    # or
    git commit -m "feat: Added new keys for amp-comp in en.json"
    ```
6.  **Push** your branch to your fork on GitHub:
    ```bash
    git push origin feature/en-json-improvement
    ```
7.  **Open a Pull Request (PR)** to the `main` branch of this repository. Describe your changes and their rationale.

## Original Source

This repository is a fork and contains translations based on the original work by:
**[CubeCoders/AMPTranslations](https://github.com/CubeCoders/AMPTranslations)**

We maintain and improve these translations for the French-speaking community (and other languages) and strive to keep up to date with changes from the original source.

## License

This project is licensed under the **MIT License**. See the [LICENSE](LICENSE) file for more details.

## Acknowledgements

A big thank you to all contributors and the AMP community for their continued work.
