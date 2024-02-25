# Documentation du Bot Discord `bot_sherlock.py`

## Description
Le bot Discord `bot_sherlock.py` est un outil basé sur l'outil de recherche d'informations `Sherlock`. Il permet aux utilisateurs de Discord de rechercher un nom d'utilisateur sur plusieurs réseaux sociaux et de récupérer des informations associées.

## Fonctionnalités

### 1. Commande `/sherlock`
   - **Description** : Recherche un nom d'utilisateur sur divers réseaux sociaux en utilisant l'outil Sherlock.
   - **Utilisation** : `/sherlock <nom_utilisateur> [--similaire]`
   - **Options** :
      - `nom_utilisateur` - Le nom d'utilisateur à rechercher.
      - `--similaire` - (Optionnel) Vérifie les noms d'utilisateur similaires en les remplaçant par des variations (par exemple, '_', '-', '.').

### 2. Commande `/help`
   - **Description** : Affiche une liste des commandes disponibles avec des détails sur l'utilisation et les options.
   - **Utilisation** : `/help`

## Utilisation
1. **Installation des dépendances** :
   - Avant d'utiliser le bot, assurez-vous d'installer les dépendances en exécutant la commande suivante :
     ```bash
     pip install discord.py
     ```

2. **Configuration** :
   - Créez un fichier `config.json` et ajoutez votre token Discord sous la clé `"discord_bot_token"`.
   - Remplacez l'ID du rôle autorisé dans le script par l'ID de votre rôle.

3. **Exécution** :
   - Exécutez le script avec la commande :
     ```bash
     python bot_sherlock.py
     ```
   
4. **Commandes Discord** :
   - Utilisez la commande `/sherlock` sur votre serveur Discord pour rechercher un nom d'utilisateur sur différents réseaux sociaux.
   - Utilisez la commande `/help` pour obtenir des informations détaillées sur les commandes disponibles.

## Remarques
- Assurez-vous que le fichier `sherlock.py` est présent dans le répertoire parent du script `bot_sherlock.py`.
- Vérifiez que le rôle spécifié dans le script correspond à celui qui devrait être autorisé à utiliser les commandes.

## Avertissement
Ce bot est basé sur l'outil open source Sherlock (https://github.com/sherlock-project/sherlock). Assurez-vous de respecter les règles d'utilisation des sites web cibles et d'obtenir les autorisations nécessaires avant d'utiliser cet outil.

---

*Remarque : Le code du bot est basé sur une version préexistante de Sherlock et est fourni à titre éducatif uniquement.*
