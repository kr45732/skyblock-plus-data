# skyblock-plus-data

## glint_images
Used for rendering the enchanted glint on items. 

## BitPrices.json
Prices for items that cost bits.
```yaml
{
  "ITEM_ID": Number,
  ...
}
```

## Constants.json
Various constants for the bot.

## CopperPrices.json
Prices for items that cost copper.
```yaml
{
  "ITEM_ID": Number,
  ...
}
```

## DragonLoot.json
Loot items and drop chances for dragons.
```yaml
{
  "dragon": {
    "Item Name": {
      "unique": Boolean,
      "quality": Number,
      "drop_chance": String,
      "eye": Boolean
    },
    ...
  }
  ...
}
```

## DungeonLoot.json
Loot items and drop chances for dungeons.
```yaml
{
  "floor": {
    "Chest": [
      {
        "item": String,
        "floor": Number,
        "chest": String,
        "cost": Number,
        "drop_chances": {
          "score": String,
          ...
        }
      },
      ...
    ],
    ...
  },
  ...
}
```

## InternalNameMappings.json
Information about all items in the game (credit to [NotEnoughUpdates-REPO](https://github.com/NotEnoughUpdates/NotEnoughUpdates-REPO)). 
```yaml
{
  "ITEM_ID": {
    "name": String,
    "recipe": {
      "slot": String,
      ...,
      "count": Number
    },
    "texture": String,
    "wiki": String,
    "scrollable": Boolean,
    "forge": Number,
    "base_rarity": String,
    "skins": [
      String,
      ...
    ],
    "npc_buy": {
      "cost": [
        String,
        ...
      ],
      "count": Number
    }
  },
  ...
}
```

## PriceOverrides.json
Manual and automatic price overrides for networth calculations.
```yaml
{
  "manual": {
    "ITEM_ID": Number,
    ...
  },
  "automatic": {
    "ITEM_ID": Number,
    ...
  }
}
```

## Settings.json
Various settings for the bot.
```yaml
{
  "mojangApiNum": Number,
  "ahApiUrl": String,
  "allowMojangApi": Boolean,
  "neuBranch": String
}
```
