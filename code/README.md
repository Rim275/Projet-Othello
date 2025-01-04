# Projet Othello 

Ce projet est une implémentation locale du jeu de société **Othello** en Java, jouable en ligne de commande. Il a été réalisé par le groupe 33, composé de :

- Nathan MUFUTA
- Selma FANANI
- Rim AMSAF
- Raissa MEZINE

# Lancer le projet Othello sans IDE

## Prérequis

1. **Java** : Assurez-vous que Java est installé sur votre machine (Java 17 ou supérieur recommandé).
    - Vous pouvez vérifier votre version de Java avec la commande suivante :
      ```bash
      java -version
      ```

2. **Gradle** :
    - Le projet inclut un wrapper Gradle, donc vous n'avez pas besoin d'installer Gradle séparément.
    - Assurez-vous que le fichier `gradlew` est exécutable (Linux/MacOS) :
      ```bash
      chmod +x gradlew
      ```

## Instructions pour exécuter le projet

### Étape 1 : Extraire le fichier ZIP

- Décompressez le fichier ZIP du projet dans un répertoire de votre choix.

### Étape 2 : Construire le projet

- Ouvrez un terminal ou un invite de commandes dans le répertoire du projet extrait.

- Utilisez le wrapper Gradle pour construire le projet :
  ```bash
  ./gradlew build  # Linux/MacOS
  gradlew.bat build  # Windows
  ```

### Étape 3 : Lancer l'application

- Une fois la construction terminée, lancez l'application avec la commande suivante :
  ```bash
  ./gradlew run  # Linux/MacOS
  gradlew.bat run  # Windows
  ```

- L'interface graphique de l'application s'ouvrira automatiquement.

## Commandes supplémentaires utiles

- **Nettoyer le projet** (supprime les fichiers générés lors de la construction) :
  ```bash
  ./gradlew clean
  ```
- **Exécuter les tests unitaires** :
  ```bash
  ./gradlew test
  ```

## Structure du projet

Voici un aperçu de la structure du projet :

```
src/
├── main/
│   ├── java/
│   │   └── fr/univ_amu/m1info/board_game_library/
│   │       ├── application/  # Logique métier
│   │       ├── controller/   # Contrôleurs et gestion d'événements
│   │       └── graphics/     # Interface graphique
│   └── resources/            # Ressources (fichiers statiques)
├── test/                     # Tests unitaires
gradle/                       # Fichiers de configuration Gradle
gradlew                       # Wrapper Gradle (Linux/MacOS)
gradlew.bat                   # Wrapper Gradle (Windows)
build.gradle                  # Configuration principale Gradle
settings.gradle               # Configuration des modules Gradle
```

## Remarque

- Si vous rencontrez des erreurs, vérifiez que votre version de Java est compatible et que toutes les dépendances nécessaires sont correctement téléchargées lors de la construction.
