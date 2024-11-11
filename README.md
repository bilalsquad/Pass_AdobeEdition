# 📚 Adobe Digital Editions Screenshot Capture Tool

## Description

Ce script **AppleScript** est conçu pour capturer automatiquement des **captures d'écran** de chaque page d'un livre protégé par **Adobe Digital Editions** sur un Mac. Il permet ainsi de générer une collection d'images représentant chaque page du livre, même si celui-ci est protégé par DRM.

> ⚠️ **Avertissement** : L'utilisation de ce script peut enfreindre les **conditions d'utilisation** d'Adobe Digital Editions et violer les **droits d'auteur**. Ce script est fourni à des fins éducatives uniquement. Assurez-vous de respecter les lois sur le droit d'auteur en vigueur dans votre pays avant de l'utiliser.

---

## 🛠️ Prérequis

- **macOS** avec l'application **AppleScript Editor** ou **Script Editor**.
- **Adobe Digital Editions** (installé sur votre Mac).
- **Accès aux préférences système** pour accorder les autorisations nécessaires (comme l'accès à l'écran).

### 📦 Installation

1. **Télécharger le script** ou copier-coller le code ci-dessous dans **AppleScript Editor**.
2. Sauvegarder le fichier sous un nom, par exemple : `CaptureScreens.scpt`.

---

## 🚀 Utilisation

### Étape 1 : Configuration initiale

1. **Ouvrez le livre** dans **Adobe Digital Editions**.
2. **Ajustez la taille de la fenêtre** pour que chaque page s'affiche complètement sans défilement.

### Étape 2 : Exécution du script

1. **Lancer le script** depuis AppleScript Editor :
   - Ouvrez le fichier `.scpt` que vous avez enregistré.
   - Cliquez sur le bouton **Exécuter**.
2. Le script commencera à capturer **chaque page** du livre.
3. **Les captures d'écran** seront sauvegardées sur le **Bureau** par défaut.

---

## 📁 Où sont sauvegardées les images ?

Les captures d'écran sont automatiquement sauvegardées dans le dossier que vous aurez choisit lors du début du script. 

## 🚑 Dépannage

1. **Erreur d'autorisation** :
   - Si le script ne fonctionne pas à cause d'un problème d'accès, allez dans :
     - **Préférences Système > Sécurité et confidentialité > Confidentialité > Accès complet au disque**
     - Ajoutez **Adobe Digital Editions** et **Script Editor** (ou **Terminal** si vous exécutez le script via le terminal).

2. **Adobe Digital Editions se fige** :
   - Si Adobe Digital Editions devient non réactif, exécutez la commande suivante dans le **Terminal** pour le relancer :
     ```bash
     killall "Adobe Digital Editions"
     ```
   - Redémarrez l'application après avoir exécuté cette commande.

3. **Le script ne passe pas à la page suivante** :
   - Vérifiez que **Adobe Digital Editions** est bien en focus lorsque le script s'exécute.
   - Essayez d'augmenter le délai entre les captures d'écran en modifiant cette ligne dans le script :
     ```applescript
     delay 0.5
     ```
     - Augmentez la valeur (par exemple, `delay 1`) pour laisser plus de temps à la page pour se charger.

4. **Les captures d'écran sont incorrectes ou incomplètes** :
   - Assurez-vous que la fenêtre **Adobe Digital Editions** est bien redimensionnée pour afficher l'intégralité de la page.
   - Vous pouvez forcer un zoom optimal en utilisant le raccourci clavier `Command + 0` avant chaque capture.

5. **Problème de compatibilité avec macOS** :
   - Ce script a été testé sur macOS Ventura. Si vous utilisez une version différente de macOS, certaines commandes peuvent nécessiter des ajustements.
   - Assurez-vous que les autorisations d'accessibilité sont accordées :
     - **Préférences Système > Sécurité et confidentialité > Confidentialité > Accessibilité**

---

## 📞 Support

Pour toute question, problème ou suggestion, n'hésitez pas à ouvrir une **Issue** sur le dépôt GitHub du projet ou à me contacter directement par email.

---

## 📃 Licence

Ce projet est sous licence **MIT**.

> **Remarque** : Ce script est fourni à des fins éducatives. Assurez-vous de respecter les lois sur le droit d'auteur et les conditions d'utilisation des logiciels que vous utilisez.



