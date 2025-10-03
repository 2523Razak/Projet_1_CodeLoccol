````
# Exercise 1

Ce projet illustre l'utilisation de commandes de base du terminal Linux pour la **création, la manipulation et la suppression de fichiers et dossiers**. Chaque étape est décrite et les commandes exécutées sont listées pour un suivi facile.

## 1. Création d'un répertoire temporaire `cli_tmp`

**Description :**  
On commence par créer un répertoire temporaire dans le répertoire personnel pour y travailler.

**Commandes exécutées :**
```bash
cd ~
mkdir cli_tmp
cd cli_tmp
````

## 2. Création de fichiers dans `cli_tmp`

**Description :**
Création de fichiers texte et d'un sous-dossier dans le répertoire temporaire.

**Commandes exécutées :**

```bash
touch je_suis_dans_tmp.txt
touch in_cli_tmp.txt
mkdir in_cli_tmp
```

## 3. Suppression d'un fichier

**Description :**
On supprime le fichier `je_suis_dans_tmp.txt`.

**Commandes exécutées :**

```bash
rm je_suis_dans_tmp.txt
```

## 4. Suppression du répertoire temporaire

**Description :**
Retour au répertoire personnel et suppression de `cli_tmp` avec tout son contenu.

**Commandes exécutées :**

```bash
cd ~
rm -r cli_tmp
```

## 5. Création de plusieurs dossiers simultanément

**Description :**
Création de plusieurs dossiers en une seule commande pour organiser la structure familiale et sociale.

**Commandes exécutées :**

```bash
mkdir grand_parent parent grand_frere grande_soeur ami connaissances
```

## 6. Déplacement d'un fichier

**Description :**
Création du fichier `bachir` dans `grand_frere` et déplacement vers le dossier `ami`.

**Commandes exécutées :**

```bash
cd grand_frere
touch bachir
mv bachir ../ami/
```

## 7. Déplacement d'un dossier

**Description :**
Déplacement du dossier `ami` dans `parent` pour organiser les dossiers.

**Commandes exécutées :**

```bash
cd ~
mv ami parent/
```

## 8. Affichage du chemin absolu

**Description :**
Afficher le chemin absolu du répertoire courant.

**Commandes exécutées :**

```bash
pwd
```