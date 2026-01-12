# Lab - Navigation par Onglets en Bas d'Écran

## 🎯 Objectif du Lab
Transformer une application React Native utilisant une Stack Navigation en une application utilisant une Bottom Tab Navigation avec React Navigation v6.

## 📋 Description
Ce laboratoire guide la configuration d'une navigation par onglets en bas d'écran (Bottom Tabs). La tâche consiste à remplacer une Stack Navigation existante par une Tab Navigation permettant de basculer entre deux écrans : Login et Welcome.

## 🏗️ Contexte Initial
Le projet contient déjà :
- Deux écrans fonctionnels : `LoginScreen` et `WelcomeScreen`
- Une navigation Stack configurée
- Tous les fichiers nécessaires sauf `App.js` qui doit être modifié

## 🎮 Fonctionnalités Requises
- Bottom Tab Navigation avec deux onglets : Login et Welcome
- Écran initial : Login
- Pas d'en-tête supplémentaire (header masqué)
- Aucune modification des autres fichiers

## 📁 Structure des Fichiers
```
.
├── App.js              ← SEUL FICHIER À MODIFIER
├── components/
│   ├── LoginScreen.js  ← Existant, ne pas modifier
│   └── WelcomeScreen.js ← Existant, ne pas modifier
└── package.json
```

## 🔧 Étapes de Réalisation

### Étape 1 : Installation
Installer la bibliothèque Bottom Tabs :
```bash
npm install @react-navigation/bottom-tabs
```

### Étape 2 : Importation
Dans `App.js`, importer `createBottomTabNavigator` et l'instancier.

### Étape 3 : Nettoyage
Supprimer toutes les références à la Stack Navigation existante.

### Étape 4 : Configuration
Configurer le Tab Navigator avec deux écrans :
- Login → LoginScreen
- Welcome → WelcomeScreen

### Étape 5 : Ajustement
Configurer les options minimales :
- Écran initial : Login
- Header masqué

## ✅ Critères de Réussite

1. **Fonctionnalité** :
   - [ ] Deux onglets fonctionnels en bas d'écran
   - [ ] Navigation entre Login et Welcome
   - [ ] Écran initial : Login

2. **Code** :
   - [ ] Seul `App.js` est modifié
   - [ ] Pas d'erreur de compilation
   - [ ] Structure React Navigation v6 correcte

3. **Interface** :
   - [ ] Onglets visibles en bas d'écran
   - [ ] Pas d'en-tête superposé
   - [ ] Interface propre et responsive

## ⚠️ Contraintes Techniques

- **React Navigation v6** obligatoire
- **Pas de personnalisation avancée** des onglets
- **Pas de modification** des écrans existants
- **Pas d'ajout** de dépendances supplémentaires

## 🐛 Problèmes Courants & Solutions

### ❌ Erreur : "NavigationContainer nested"
**Cause** : Double `NavigationContainer` dans l'application
**Solution** : Vérifier qu'un seul `NavigationContainer` existe

### ❌ Erreur : Onglets non visibles
**Cause** : Problème de style ou de structure
**Solution** : Vérifier la flexibilité des conteneurs

### ❌ Erreur : "Module not found"
**Cause** : @react-navigation/bottom-tabs non installé
**Solution** : `npm install @react-navigation/bottom-tabs`

## 📱 Résultat Final Attendus

### Comportement :
1. L'application démarre sur l'écran Login
2. Une barre d'onglets en bas permet de switcher entre :
   - Onglet "Login" → Affiche LoginScreen
   - Onglet "Welcome" → Affiche WelcomeScreen
3. Pas d'en-tête visible au-dessus des écrans

### Interface :
```
+-------------------+
|                   |
|                   |
|    Contenu de     |
|     l'écran       |
|                   |
|                   |
|                   |
+-------------------+
|  Login | Welcome  |
+-------------------+
```

## 🔍 Validation

Pour valider votre implémentation :

1. **Test visuel** :
   - Vérifiez la présence des deux onglets
   - Testez la navigation entre les écrans
   - Vérifiez l'absence d'en-tête

2. **Test technique** :
   ```bash
   npm start
   # L'application doit se compiler sans erreur
   # La navigation doit être fluide
   ```

3. **Test de conformité** :
   - Ouvrez `App.js` et vérifiez qu'aucun autre fichier n'a été modifié
   - Vérifiez que seules les étapes demandées sont implémentées

## 📚 Concepts Clés Maîtrisés

À l'issue de ce lab, vous devez comprendre :
- La différence entre Stack et Tab Navigation
- La configuration de base de React Navigation v6
- L'instanciation et l'utilisation de `createBottomTabNavigator`
- Les options de configuration minimales d'un navigateur

## Démonstration

<img width="959" height="473" alt="LAB10 1" src="https://github.com/user-attachments/assets/80e436b2-4388-475d-8e70-80a14931dd76" />



## 🏆 Compétences Évaluées

- [ ] Installation correcte des dépendances
- [ ] Importation des modules nécessaires
- [ ] Configuration du Bottom Tab Navigator
- [ ] Déclaration des écrans dans les onglets
- [ ] Gestion des options de navigation
- [ ] Respect des contraintes du lab

## Auteurs 

Réalisé par : Ettouyjer yasmine

Encadré par : Pr.Mohamed Lechgar.
