# Bienvenue sur MCP Docs.

## Prérequis

* [MCP Reborn](https://github.com/Hexeption/MCP-Reborn/releases)
* [OpenJDK 8](https://adoptopenjdk.net/)
* [Eclipse](https://www.eclipse.org/downloads/packages/release/2021-03/r/eclipse-ide-java-developers) ou [Intellij](https://www.jetbrains.com/fr-fr/idea/download/)


C'est bon vous avez tout ?
Bon on peut commencer.

## Importer le projet

En premier lieu il faudra que vous aiez dézippé MCP-Reborn dans un dossier.

Ensuite il faut importer le projet dans votre ide.

Pour [Eclipse](https://youtu.be/tS0WTf5bsVU?t=18).
Pour [Intellij](https://www.youtube.com/watch?v=wQyDk4Ji1Gk=)

Dès que tout cela est fait vous devrez ouvrir un cmd à l'emplacement où vous avez dézippé MCP et écrire la commande suivante : 
```BASH
gradlew setup
```

Créez un package pour que l'on puisse un peu mieux différencier le code de Minecraft et le votre.

```
| src/main/java
| net.minecraft
| com.mojang
| mcp
| votre package
```

Pour lancer le jeu vous devrez executer la commande suivante ```gradlew runclient```