# Objectifs du projet

Ce projet a pour but d'apprendre à utiliser le terminal (CLI – Command Line Interface).  
À travers plusieurs exercices, nous allons :

1. Comprendre ce qu'est un terminal et pourquoi l'utiliser.
2. Apprendre à se déplacer dans les dossiers à l'aide de commandes simples.
3. Créer, déplacer, renommer et supprimer des dossiers et fichiers.
4. Découvrir les fichiers cachés et leur importance.
5. Développer de bonnes habitudes pour organiser son environnement numérique.


# Exercice 1

## Commandes exécutées :

```bash
cd ~
mkdir cli_tmp
cd cli_tmp
touch je_suis_dans_tmp.txt
touch in_cli_tmp.txt
mkdir in_cli_tmp
rm je_suis_dans_tmp.txt
cd ~
rm -r cli_tmp
mkdir grand_parent parent grand_frere grande_soeur ami connaissances
cd grand_frere
touch bachir
mv bachir ../ami/
cd ~
mv ami parent/
pwd
```

## Explication :

- `cd ~` : aller dans le dossier personnel.  
- `mkdir` : créer un dossier.  
- `touch` : créer un fichier vide.  
- `rm` : supprimer un fichier.  
- `rm -r` : supprimer un dossier et son contenu.  
- `mv` : déplacer ou renommer un fichier.  
- `pwd` : afficher le chemin complet du dossier actuel.

### Difficultés rencontrées :

Au début, la différence entre `rm` et `rm -r` n'était pas évidente. Il faut retenir que `rm` sert pour les fichiers et `rm -r` pour les dossiers.

# Exercice 2

## Commandes exécutées :

```bash
cd ~
mkdir conteneur
cd conteneur
mkdir voitures ustensiles electronique

cd voitures
echo "benz" > mes_voitures.txt
echo "toyota" >> mes_voitures.txt
echo "honda" >> mes_voitures.txt

cd ../ustensiles
echo "cuillere" > cuisine.txt
echo "marmite" >> cuisine.txt
echo "couteau" >> cuisine.txt

cat cuisine.txt
cd ..
ls -l
```

## Explication :

- `echo "texte"` : écrire du texte dans un fichier.  
- `>` : créer un fichier et écrire dedans.  
- `>>` : ajouter du texte sans effacer l'ancien contenu.  
- `cat` : afficher le contenu d'un fichier.  
- `ls -l` : lister les fichiers et dossiers avec des détails.

## Difficultés rencontrées :

Il fallait faire attention à ne pas utiliser `>` à la place de `>>`, sinon on écrasait le fichier.

# Exercice 3

## Commandes exécutées :

```bash
mkdir -p actualites/politique
cd actualites/politique
mkdir elections
cd elections
echo "Issoufou" > candidats.txt
echo "Hama" >> candidats.txt
echo "Seini" >> candidats.txt
cd ../..
mkdir buzz
```

## Explication :

- `mkdir -p` : permet de créer plusieurs dossiers en une seule commande.  
- `cd ../..` : remonter de deux dossiers vers l'arrière.

## Difficultés rencontrées :

Il fallait bien comprendre comment `..` fonctionne. Chaque `..` fait remonter d'un dossier.

# Exercice 4

## Commandes exécutées :

```bash
cd ~
touch .configuration
ls -a

mkdir -p creations/crayons
cd creations/crayons
touch couleurs.txt
mv couleurs.txt colors.txt

cd ..
touch gomme.txt
mv gomme.txt crayons/
cd ~
```

## Explication :

- Un fichier commençant par un point (`.`) est caché.  
- `ls -a` : permet d'afficher les fichiers cachés.  
- `mv` : sert à renommer ou déplacer un fichier.

# Exercice 5

## Commandes exécutées :

```bash
mkdir -p projet_scolaire/maths projet_scolaire/sciences

cd projet_scolaire/maths
echo "x^2 + y^2 = z^2" > equations.txt

cd ../sciences
echo "eau + huile = séparation" > experiences.txt

cd ../maths
mv equations.txt geometrie.txt

cd ../sciences
mv experiences.txt ../maths/

cd ..
rmdir sciences
```

## Explication :

- `rmdir` : supprime un dossier vide.  
- On apprend ici à renommer et déplacer des fichiers entre dossiers.

## Difficultés rencontrées :

Un dossier doit être vide avant d'être supprimé avec `rmdir`.


# Exercice 6

## Commandes exécutées :

```bash
mkdir votrenom
cd votrenom

touch banque.txt sante.txt .mdp
echo "Relevé bancaire janvier" > banque.txt
echo "Vaccination complète" > sante.txt

ls -a
mv sante.txt medical.txt
mkdir documents
mv banque.txt medical.txt documents/
rm .mdp
```

## Explication :

- `.mdp` est un fichier caché (souvent pour des informations sensibles).  
- `rm` permet de le supprimer une fois qu'il n'est plus utile.  
- `mv` sert à organiser les fichiers dans un dossier.

## Difficultés rencontrées :

Il ne faut pas oublier de mettre un point au début du nom pour créer un fichier caché.


# Difficultés générales

- Confusion entre `cd` (changer de dossier) et `mkdir` (créer un dossier).  
- Mauvaise utilisation de `>` à la place de `>>`.  
- Erreurs lors de la suppression de dossiers non vides.  
- Oublier de revenir dans le bon dossier avant d'exécuter une commande.

Ces exercices ont permis de mieux comprendre le fonctionnement du terminal et de la ligne de commande.  
Ils montrent l'importance d'une bonne organisation dans un système de fichiers et d'une bonne utilisation des commandes de base.  
Le terminal est un outil puissant qui, une fois compris, permet de travailler plus rapidement et plus efficacement.
