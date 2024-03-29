# Documentation du Bot Discord `bot_search.py`

## Description
Le bot Discord `bot_search.py` est un assistant polyvalent qui intègre des fonctionnalités de recherche en ligne et d'analyse de liens. Grâce à l'utilisation de Discord.py et Pyppeteer, le bot offre une expérience interactive, permettant aux utilisateurs de Discord d'effectuer des recherches sur Google, de prendre des captures d'écran de sites web, et d'analyser des liens spécifiques avec VirusTotal.

## Fonctionnalités

### 1. Commande `/google`
   - **Description** : Effectue une recherche sur Google et retourne les liens pertinents ainsi que des captures d'écran des sites correspondants.
   - **Utilisation** : `/google <query> [result_count]`
   - **Exemple** : `/google python programming 5`
   - **Résultats** : Le bot renvoie des liens pertinents liés à la requête Google et fournit des captures d'écran pour visualiser les sites associés.

### 2. Commande `/googlesite`
   - **Description** : Prend une capture d'écran du site web spécifié.
   - **Utilisation** : `/googlesite <url>`
   - **Exemple** : `/googlesite https://www.example.com`
   - **Résultats** : Le bot capture une image du site web fourni et l'affiche dans le canal Discord.

### 3. Commande `/vt4`
   - **Description** : Analyse un lien pour détecter les menaces à l'aide de VirusTotal et fournit des informations détaillées ainsi qu'une capture d'écran du rapport.
   - **Utilisation** : `/vt4 <link>`
   - **Exemple** : `/vt4 https://www.example.com`
   - **Résultats** : Le bot analyse le lien avec VirusTotal, extrait des informations détaillées, et fournit une capture d'écran du rapport pour une évaluation visuelle.

## Utilisation
1. **Installation des dépendances** :
   - Avant d'utiliser le bot, assurez-vous d'installer les dépendances en exécutant la commande suivante :
     ```bash
     pip install discord.py aiohttp beautifulsoup4 googlesearch-python Pillow pyppeteer pyppeteer_stealth
     ```

2. **Configuration** :
   - Créez un fichier `config.json` et ajoutez votre token Discord sous la clé `"discord_bot_token"`.

3. **Exécution** :
   - Exécutez le script avec la commande :
     ```bash
     python bot_search.py
     ```
   
4. **Commandes Discord** :
   - Utilisez les commandes `/google`, `/googlesite`, et `/vt4` sur votre serveur Discord pour tirer parti des fonctionnalités du bot.

## Remarques
- Le bot nécessite l'installation de Google Chrome et le chemin vers l'exécutable de Chromium doit être spécifié dans le script (`chromium_path`).
- Assurez-vous que le bot dispose des autorisations nécessaires sur votre serveur Discord pour exécuter les commandes spécifiées dans le script.
