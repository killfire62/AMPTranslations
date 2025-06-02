* 🇫🇷 [Français](#amptranslations--fichiers-de-localisation-multi-langues-pour-amp)
* 🇬🇧 [English](#amptranslations-multi-language-localization-files-for-amp)

---

# AMPTranslations : Fichiers de Localisation Multi-Langues pour AMP

Ce dépôt fournit des fichiers de traduction (`.json`) pour divers composants et fonctionnalités **AMP (Accelerated Mobile Pages)** dans plusieurs langues, notamment le **français (fr.json)**, l'**anglais (en.json)**, l'**allemand (de.json)**, l'**espagnol (es.json)** et le **polonais (pl.json)**.

## Comment Utiliser ces Traductions

Pour intégrer ces traductions dans votre page AMP :

1.  **Téléchargez les fichiers de langue souhaités :**
    Cliquez sur les liens ci-dessous pour télécharger directement les fichiers :
    * [Français (fr.json)](https://raw.githubusercontent.com/killfire62/AMPTranslations/main/fr.json)
    * [Anglais (en.json)](https://raw.githubusercontent.com/killfire62/AMPTranslations/main/en.json)
    * [Allemand (de.json)](https://raw.githubusercontent.com/killfire62/AMPTranslations/main/de.json)
    * [Espagnol (es.json)](https://raw.githubusercontent.com/killfire62/AMPTranslations/main/es.json)
    * [Polonais (pl.json)](https://raw.githubusercontent.com/killfire62/AMPTranslations/main/pl.json)

2.  **Placez les fichiers de traduction dans le répertoire Locale :**
    Copiez les fichiers `.json` téléchargés dans le répertoire `Locale` de votre environnement AMP, par exemple :
    `home\amp\.ampdata\instances\ADS01\WebRoot\Locale\`

3.  **Appliquez les traductions via le paramètre d'URL :**
    Une fois les fichiers `.json` placés dans le répertoire `Locale`, le système AMP peut les charger automatiquement en fonction du paramètre `lang` dans l'URL.
    **Exemple pour le français :**
    `http://votre-adresse-ip-ou-domaine-amp:port/?lang=fr`
    (Remplacez `votre-adresse-ip-ou-domaine-amp:port` par l'IP ou le domaine de votre serveur AMP et le port si nécessaire.)

## Composants et Langues Disponibles

Ce dépôt contient des fichiers de traduction pour les langues suivantes :

* **Français** (`fr.json`)
* **Anglais** (`en.json`)
* **Allemand** (`de.json`)
* **Espagnol** (`es.json`)
* **Polonais** (`pl.json`)

Chaque fichier contient des traductions pour diverses chaînes de caractères utilisées par les composants et le runtime AMP. Examinez les fichiers `.json` pour voir les clés de traduction spécifiques et leur contenu.

## Source Originale / Original Source

Ce dépôt est un fork et contient des traductions basées sur le travail original de :
**[CubeCoders/AMPTranslations](https://github.com/CubeCoders/AMPTranslations)**

---

<br>
<br>

# AMPTranslations: Multi-Language Localization Files for AMP

* [Français](#amptranslations--fichiers-de-localisation-multi-langues-pour-amp)
* [English](#amptranslations-multi-language-localization-files-for-amp)

---

This repository provides translation files (`.json`) for various **AMP (Accelerated Mobile Pages)** components and features in multiple languages, including **French (fr.json)**, **English (en.json)**, **German (de.json)**, **Spanish (es.json)**, and **Polish (pl.json)**.

## How to Use These Translations

To integrate these translations into your AMP page:

1.  **Download the desired language files:**
    Click on the links below to directly download the files:
    * [French (fr.json)](https://raw.githubusercontent.com/killfire62/AMPTranslations/main/fr.json)
    * [English (en.json)](https://raw.githubusercontent.com/killfire62/AMPTranslations/main/en.json)
    * [German (de.json)](https://raw.githubusercontent.com/killfire62/AMPTranslations/main/de.json)
    * [Spanish (es.json)](https://raw.githubusercontent.com/killfire62/AMPTranslations/main/es.json)
    * [Polish (pl.json)](https://raw.githubusercontent.com/killfire62/AMPTranslations/main/pl.json)

2.  **Place the translation files in the Locale directory:**
     Copy the downloaded `.json` files into the `Locale` directory of your AMP environment, for example:
     `home\amp\.ampdata\instances\ADS01\WebRoot\Locale\`

3.  **Apply translations via URL parameter:**
    Once the `.json` files are placed in the `Locale` directory, the AMP system can load them automatically based on the `lang` parameter in the URL.
    **Example for English:**
    `http://your-amp-server-ip-or-domain:port/?lang=en`
    (Replace `your-amp-server-ip-or-domain:port` with your AMP server's IP or domain and port if needed.)

## Available Components and Languages

This repository contains translation files for the following languages:

* **French** (`fr.json`)
* **English** (`en.json`)
* **German** (`de.json`)
* **Spanish** (`es.json`)
* **Polish** (`pl.json`)

Each file contains translations for various strings used by AMP components and the AMP runtime. Examine the `.json` files to see the specific translation keys and their content.

## Original Source

This repository is a fork and contains translations based on the original work by:
**[CubeCoders/AMPTranslations](https://github.com/CubeCoders/AMPTranslations)**
