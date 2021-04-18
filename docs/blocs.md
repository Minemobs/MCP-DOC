## Comment créer un block

Allez dans le package net.minecraft.block puis dans la classe Blocks.
Cette dernière sert à initializer des blocs.

Voici un exemple de bloc simple:
```Java
   public static final Block TEST_BLOCK = register("test_block", new Block(Block.Properties.from(Blocks.STONE).sound(SoundType.WOOD).zeroHardnessAndResistance()));
```

Ensuite il faudra faire créer un BlockItem. Cela permet d'avoir l'item dans notre inventaire.
Il faut que vous alliez dans le package net.minecraft.item puis dans la classe Items.

Exemple:
```Java
public static final Item TEST_BLOCK = register(Blocks.TEST_BLOCK);
```

Voilà vous avez crée votre propre bloc.

Passons aux explications:
Tout comme la fonction register pour les items cette dernière prend en paramètres le nom du bloc et ses propriétés.

``Block.Properties.from`` signifie que l'on va copier les propriétés du bloc de Stone.

La fonction ``zeroHardnessAndResistance`` donne aucune résistance à notre bloc. C'est comme avec le bloc de tnt il se casse très rapidement.

La fonction ``register`` de la classe Items prend en paramètre le bloc auquel on souhaite donner un item.

--------------

## Vidéos Youtube

<iframe width="560" height="315" src="https://www.youtube.com/embed/dVsA9y9nBX8" title="Tutoriel créer un block avec MCP Reborn" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

<iframe width="560" height="315" src="https://www.youtube.com/embed/JR0mGzEnnoA" title="Tutoriel MCP par KinderrKill" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>