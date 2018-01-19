# Outils et configuration pour Eclipse

## Snippets Oracle SQL

- add column if not exists
- safe_add_constraint_FK
- safe_create_table
- safe_delete_index
- safe_drop_something
- safe_insert

## Plugins indispensables

### EclEmma Java Code Coverage

> Anaylse de couverture de code intégré à Eclipse

[Marketplace](http://marketplace.eclipse.org/content/eclemma-java-code-coverage)

- Ajouter la vue : __Windows__ / __Show view__ / __Other ...__ / __Coverage__
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

