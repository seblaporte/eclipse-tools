# Outils et configuration pour Eclipse

## Configuration d'Eclipse

Sous Windows, la configuration d'Eclipse s'effectue depuis : __Window__ / __Preferences__

### Modification de l'indentation

- Aller dans Java / Code Style / Formatter : Cliquer sur __Edit...__
- Dans l'onglet __Indentation__ / partie __General settings__ / Sélectionner __Spaces only__ pour __Tab Policy__
- Dans l'onglet __Line Wrapping__ / partie __Settings for arguments__ / Sélectionner _Wrap all elements, every element on a new line_ pour __Line wrapping policy__

### Activer et configurer les Save Actions

- Aller dans Java / Editor / Save Actions
- Cocher _Perform the selected actions on save__ avec _Additional actions_
- Cliquer sur __Configure__ :
  * Dans __Code Organizing__ :
    - Cocher _Remove trailing withspace_ avec _All lines_
    - Cocher _Correct indentation_
  * Dans __Code Style__ :
    - Cocher _Use blocks in if/while/for/do statements_ avec _Always_
  * Dans __Unnecessary Code__
    - Cocher _Remove unused imports_
    - Cocher _Remove unused private members_ avec _Types_ et _Constructors_
    - Cocher _Remove unnecessary casts_
    - Cocher _Remove redundant type arguments (1.7 or higher)_

### Visualiser l'utilisation mémoire d'Eclipse

Visualisation de l'utilisation mémoire, dans les préférences : __General__ / cocher __Show heap status__

### Modification de la couleur de surlignage des occurences (jaune souvent trop peu visible)

__General__ / __Editors__ / __Text Editors__ / __Annotations__ / dans __Annotation types__ / Sélectionner __Occurences__ / sur la droite __Color__

## La vue Package Explorer

La vue Package Explorer remplace avantageusement la vue Projet Explorer, par défaut à gauche. Elle permet de classifier les projets dans des Java Working Sets

Pour l'ajouter : __Window__ / __Show view__ / __Other ...__ / __Package Explorer__

La petite flèche en haut à droite de la vue permet de mettre les Working Sets comme éléments racines : __Top Level Elements__ / __Working Sets__

Pour ajouter un Working Set : __File__ / __New__ / __Other ...__ / __Java Working Set__

## Snippets Oracle SQL

> Requiert l'installation du plugin __SQL Developement Tools__ (Voir ci-dessous)

### Import des snippets

- Aller dans les préférences : Data Management / SQL Developement / SQL Editor / Templates
- Cliquer sur __Import...__ et sélectionner le fichier __Snippets_Oracle_SQL.xml__

### Snippets disponibles

- add column if not exists
- safe_add_constraint_FK
- safe_create_table
- safe_delete_index
- safe_drop_something
- safe_insert

## Plugins indispensables

### Subversive

SubVersive est un plugin qui permet de brancher votre gestionnaire de sources (Git ou SVN) à Eclipse, et donc de gérer directement vos update, commit, revert, conflits, etc. dans Eclipse. Il comprend aussi une perspective de synchronisation.

Se rendre à la perspective de synchronisation : __Window__ / __Perspective__ / __Open Perspective__ / __Other ...__ / __Team Synchronizing__

[Marketplace](https://marketplace.eclipse.org/content/subversive-svn-team-provider)

### EclEmma Java Code Coverage

> Anaylse de couverture de code intégré à Eclipse

[Marketplace](http://marketplace.eclipse.org/content/eclemma-java-code-coverage)

- Ajouter la vue : __Window__ / __Show view__ / __Other ...__ / __Coverage__
- Configurer l'analyse :
	* Clique droit sur le projet : __Coverage As__ / __Coverage Configurations...__
	* Nouvelle configuration Junit :
		- Dans l'onglet __Test__ : Run all tests in the selected project [...] et cliquer sur __Search__ : `src/test/java`
		- Dans l'onglet __Coverage__ : Sélectionner uniquement les packages nécesaires pour l'analyse

### Infinitest

> Relance automatiquement les tests Junit et permet d'identifier la ligne de code qui fait échouer le test

[Marketplace](http://marketplace.eclipse.org/content/infinitest)

### SQL Developement Tools

> Propose la connexion à des bases de données SQL et les outils nécessaire à l'éecriture de scripts.

[Marketplace](http://marketplace.eclipse.org/content/sql-development-tools)

### Complete Current Statement

> Ajoute un fonctionnalité présente dans IntelliJ pour l'auto-completion avec le raccourci `Ctrl + Shift + Enter`

__Installation__ :

- Aller dans __Help__ / __Install New Software__
- Ajouter l'url `https://github.com/henri5/completeline-updatesite/raw/master/`

### JAutodoc

> Génère automatiquement la document des méthodes en fonction de la signature

[Marketplace](http://marketplace.eclipse.org/content/jautodoc)
