![Java CI with Maven](https://github.com/Nonorc/whiteapp-mvc/workflows/Java%20CI%20with%20Maven/badge.svg?branch=master)[![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=${{secrets.SONAR_PROJECT_KEY}}&metric=alert_status)](https://sonarcloud.io/dashboard?id=Nonorc_whiteapp-mvc)[![codecov](https://codecov.io/gh/Nonorc/whiteapp-mvc/branch/master/graph/badge.svg)](https://codecov.io/gh/Nonorc/whiteapp-mvc)

# WhiteApp

Exemple architectural de projet avec les technologies Java EE.

Ce projet est sous licence **CeCILL** (**CE**A **C**NRS **I**NRIA **L**ogiciel **L**ibre),
une licence de logicielle libre compatible avec la **GNU GPL**.

> En savoir plus sur la licence [CeCILL](http://cecill.info/index.fr.html)

## Module

Ce projet ce compose d'un seul module de type **WAR** *(Web ARchive)*.
   
## Architecture

L’architecture logicielle mise en place est **MVC** *(Model View Controller)*.

* *Model*
    * Représente les données métiers et les fonctions de persistance.
* *Controller*
    * Représente la logique de traitement et la gestion des exceptions.
* *View*
    * Représente la partie graphique permettant l’interaction humaine avec l'application.

## Environnement

Ce projet est réalisé en **Java 11** *(OpenJDK)*, **JavaEE 8** et **Payara 5.201**.
Il utilise l'outil **Maven** en version 3.6.2.

### Exécution

Récupération du projet:
~~~
    git clone https://github.com/ZelmoTheDragon/whiteapp-mvc.git
    mvn install
~~~

Exécution du projet:
~~~
    mvn payara-micro:start
~~~

Puis accéder à l'adresse:
~~~
http://localhost:8080/whiteapp
~~~
