# Documentation du Bot Discord `bot_protection.js`

## Description
Le bot Discord `bot_protection.js` est un bot multifonction qui offre des fonctionnalités de protection de l'anonymat et de suppression automatique des messages sur certains canaux. Il utilise Discord.js et propose des commandes pour configurer la protection des pseudonymes des membres ainsi que la suppression automatique des messages dans des canaux spécifiques.

## Fonctionnalités

### 1. Protection de l'anonymat
   - **Commande** : `/protect`
   - **Description** : Active la protection de l'anonymat dans un canal spécifié en changeant les pseudonymes des membres pour rester anonyme et sécurisé.
   - **Utilisation** : `/protect <channel_id>`
   - **Exemple** : `/protect 123456789012345678`
   - **Résultats** : Le bot réagit avec 🔒 sur un message dans le canal spécifié. Les membres qui réagissent avec 🔒 auront leur pseudonyme changé pour une chaîne vide, les maintenant anonymes.

### 2. Configuration de la suppression automatique des messages
   - **Commande** : `/autodelete setup`
   - **Description** : Configure la suppression automatique des messages dans un canal spécifié après un certain laps de temps.
   - **Utilisation** : `/autodelete setup`
   - **Résultats** : Le bot vous guide pour mentionner le canal et spécifier le temps après lequel tous les messages seront supprimés.

### 3. Suppression immédiate des messages
   - **Commande** : `/deletenow`
   - **Description** : Supprime tous les messages dans un canal spécifié.
   - **Utilisation** : `/deletenow <channel_id>`
   - **Exemple** : `/deletenow 123456789012345678`
   - **Résultats** : Le bot supprime tous les messages non épinglés dans le canal spécifié.

## Utilisation
1. **Installation des dépendances** :
   - Installez les dépendances nécessaires en exécutant la commande suivante :
     ```bash
     npm install discord.js
     ```

2. **Configuration** :
   - Modifiez le fichier du script pour spécifier votre jeton Discord (`token`), préfixe (`prefix`), et autres configurations si nécessaire.

3. **Exécution** :
   - Exécutez le script avec la commande :
     ```bash
     node bot_protection.js
     ```
   
4. **Commandes Discord** :
   - Utilisez les commandes spécifiées dans le script sur votre serveur Discord pour bénéficier des fonctionnalités du bot.

## Remarques
- Assurez-vous que le bot dispose des autorisations nécessaires sur votre serveur Discord pour exécuter les commandes spécifiées dans le script.
- Le fichier de configuration `config.json` est utilisé pour stocker les configurations de suppression automatique des messages.

---

*Note : Vous devez remplacer les valeurs de jeton, préfixe, et autres configurations dans le script avant de l'exécuter.*
