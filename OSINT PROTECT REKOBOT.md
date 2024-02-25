```markdown
# Documentation du Bot Discord `rekognition-bot.py`

```
# Bot Discord d'analyse de photos et de comparaison de visages par RocketGod
# https://github.com/RocketGod-git/rekognition-bot

## Description
Le bot Discord `rekognition-bot.py` est un assistant qui utilise Amazon Rekognition pour analyser des photos, détecter des objets, reconnaître des célébrités, effectuer une analyse faciale, et comparer des visages. Il permet aux utilisateurs de Discord d'obtenir des informations détaillées sur des photos spécifiques, y compris la détection d'objets, la reconnaissance de célébrités, et l'analyse faciale.

## Fonctionnalités

### 1. Commande `/photos`
   - **Description** : Analyse une photo pour détecter des objets, reconnaître des célébrités, effectuer une analyse faciale, et éventuellement comparer des visages sur deux photos.
   - **Utilisation** : `/photos <première_photo> [deuxième_photo]`
   - **Exemple** : `/photos [attacher une image] [attacher une autre image]`
   - **Résultats** : Le bot renvoie un message avec des informations détaillées sur les objets détectés, les célébrités reconnues, les émotions faciales, et la similarité entre les visages si deux photos sont fournies.

## Utilisation
1. **Installation des dépendances** :
   - Avant d'utiliser le bot, assurez-vous d'installer les dépendances en exécutant la commande suivante :
     ```bash
     pip install discord boto3
     ```

2. **Configuration** :
   - Créez un fichier `config.json` et ajoutez votre token Discord, ainsi que les clés d'accès AWS sous les clés `"TOKEN"`, `"AWS_ACCESS_KEY"`, et `"AWS_SECRET_KEY"`.

3. **Exécution** :
   - Exécutez le script avec la commande :
     ```bash
     python rekognition-bot.py
     ```
   
4. **Commandes Discord** :
   - Utilisez la commande `/photos` sur votre serveur Discord pour analyser et comparer des photos.

## Remarques
- Assurez-vous que le bot dispose des autorisations nécessaires sur votre serveur Discord pour exécuter les commandes spécifiées dans le script.
- Pour utiliser la comparaison de visages, assurez-vous que votre compte AWS a l'accès approprié à Amazon Rekognition.
