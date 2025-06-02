<!-- Liens de navigation -->
<p align="right">
  <a href="#french"><img src="https://upload.wikimedia.org/wikipedia/commons/6/6a/Drapeau_France.png" alt="Français" width="20"/> Français</a> |
  <a href="#english"><img src="https://upload.wikimedia.org/wikipedia/commons/a/ae/Flag_of_the_United_Kingdom.svg" alt="English" width="20"/> English</a>
</p>

---

# AMPTranslations : Fichiers de Localisation Multi-Langues pour AMP

![Statut de Traduction](https://img.shields.io/badge/statut-active-blue)

## Sommaire

- [Comment Utiliser ces Traductions](#comment-utiliser-ces-traductions)
- [Composants et Langues Disponibles](#composants-et-langues-disponibles)
- [Source Originale](#source-originale)
- [Remerciements](#remerciements)

---

## Comment Utiliser ces Traductions

Pour intégrer ces traductions dans votre page AMP :

1. **Téléchargez les fichiers de langue souhaités :**
   * [Français (fr.json)](https://raw.githubusercontent.com/killfire62/AMPTranslations/main/fr.json)
   * [Anglais (en.json)](https://raw.githubusercontent.com/killfire62/AMPTranslations/main/en.json)
   * [Allemand (de.json)](https://raw.githubusercontent.com/killfire62/AMPTranslations/main/de.json)
   * [Espagnol (es.json)](https://raw.githubusercontent.com/killfire62/AMPTranslations/main/es.json)
   * [Polonais (pl.json)](https://raw.githubusercontent.com/killfire62/AMPTranslations/main/pl.json)

2. **Placez les fichiers de traduction dans le répertoire `Locale` :**

   Copiez les fichiers `.json` téléchargés dans le dossier suivant sur votre serveur AMP (Linux) :

   `/home/amp/.ampdata/instances/ADS01/WebRoot/Locale/`

3. **Appliquez la langue via le paramètre d’URL :**  
   Une fois les fichiers en place, utilisez le paramètre `lang` dans l’URL pour charger la langue souhaitée.

   Exemple pour le français :  
   `http://votre-adresse-ip-ou-domaine-amp:port/?lang=fr`

---

## Composants et Langues Disponibles

Ce dépôt contient des fichiers de traduction pour les langues suivantes :

- **Français** (`fr.json`)
- **Anglais** (`en.json`)
- **Allemand** (`de.json`)
- **Espagnol** (`es.json`)
- **Polonais** (`pl.json`)

Chaque fichier couvre les chaînes utilisées par les composants et le système AMP. Consultez les fichiers pour voir les clés et leur contenu.

---

## Source Originale

Ce dépôt est un fork et s'appuie sur le travail original de :  
**[CubeCoders/AMPTranslations](https://github.com/CubeCoders/AMPTranslations)**

---

## Remerciements

Un grand merci à tous les contributeurs et à la communauté AMP pour leur soutien continu.

---

<br><br>

---

# AMPTranslations: Multi-Language Localization Files for AMP
<p id="english"></p>

![Translation Status](https://img.shields.io/badge/status-active-blue)

## Table of Contents

- [How to Use These Translations](#how-to-use-these-translations)
- [Available Components and Languages](#available-components-and-languages)
- [Original Source](#original-source)
- [Acknowledgements](#acknowledgements)

---

## How to Use These Translations

To integrate these translation files into your AMP instance:

1. **Download the desired language files:**
   * [French (fr.json)](https://raw.githubusercontent.com/killfire62/AMPTranslations/main/fr.json)
   * [English (en.json)](https://raw.githubusercontent.com/killfire62/AMPTranslations/main/en.json)
   * [German (de.json)](https://raw.githubusercontent.com/killfire62/AMPTranslations/main/de.json)
   * [Spanish (es.json)](https://raw.githubusercontent.com/killfire62/AMPTranslations/main/es.json)
   * [Polish (pl.json)](https://raw.githubusercontent.com/killfire62/AMPTranslations/main/pl.json)

2. **Place the `.json` files into the `Locale` directory:**

   Copy the downloaded files into the following directory on your AMP server (Linux):

   `/home/amp/.ampdata/instances/ADS01/WebRoot/Locale/`

3. **Apply the language using the `lang` parameter in the URL:**

   Example for English:  
   `http://your-amp-server-ip-or-domain:port/?lang=en`

---

## Available Components and Languages

This repository contains translations for the following languages:

- **French** (`fr.json`)
- **English** (`en.json`)
- **German** (`de.json`)
- **Spanish** (`es.json`)
- **Polish** (`pl.json`)

Each file provides strings for AMP components and runtime. Explore the JSON files to view all keys and values.

---

## Original Source

This repository is a fork based on the original work by:  
**[CubeCoders/AMPTranslations](https://github.com/CubeCoders/AMPTranslations)**

---

## Acknowledgements

Many thanks to all contributors and the AMP community for their ongoing support.
