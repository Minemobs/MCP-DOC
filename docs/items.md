## Comment créer un item 

Allez dans le package net.minecraft.items et cherchez la classe Items.
Cette classe sert à initializer des Items.
Allez tout en bas et créez votre item. Je vous conseille de regarder l'exemple ci-dessous ou de regarder un item basique comme le bâton.

```Java
public static final Item TEST_ITEM = register("test_item", new Item(new Item.Properties().group(ItemGroup.TOOLS)));
```

Ensuite démarrez votre jeu en faisant ```gradlew runclient``` dans votre cmd

Maintenant si vous effectuez la commande ```/give @s minecraft:test_item``` vous aurez votre item dans votre inventaire.

Passons aux explications:

La fonction register prend 2 paramètres en compte. Le nom de l'item (Il doit toujours être en minuscule et ne pas avoir d'espace) et l'item.

La constructeur Item demande des propriétés pour l'item.

La fonction group met l'item dans un Creative Tab.

--------------

## Vidéos Youtube

<iframe width="560" height="315" src="https://www.youtube.com/embed/lfdvOVq5Kd0" title="Tutoriel Yotutube créer un block" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
