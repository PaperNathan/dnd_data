# Utility Types
Some types will be valuable across a lot of different objects.  It will be valuable to store them here.

# Books
```ts
type SourceBooksAbbr =  "AI" | "BomT" | "DMG" | "EGtW" | "ERLW" | "EEPC" | "FToD" | "GGtR" | "GotG" | "ID:RotF" | "KGV" | "LR" | "MM" | "MMoM" | "MOoT" | "MToF" | "OGA" | "PB:SO" | "PaitM" | "PHB" | "SAiS" | "SCAG" | "SCoC" | "SotDQ" | "TCoE" | "ToD" | "VGtM" | "WBtW" | "WGtE" | "XGtE";

type SourceBooks = "Aquisitions Incorporated" | "The Book of Many Things" | "Dungeon Master's Guide" | "Explorer's Guide to Wildemount" | "Eberron: Rising From the Last War" | "Elemental Evil Player's Companion" | "Fizban's Treasure of Dragons" | "Guildmasters' Guide to Ravnica" | "Bigby Presents: Glory of the Giants" | "Icewind Dale: Rime of the Frostmaiden" | "Keys from the Golden Vault" | "Locathah Rising" | "Monster Manual" | "Mordenkainen Presents: Monsters of the Multiverse" | "Mystic Odysseys of Theros" | "Mordenkainen's Tome of Foes" | "One Grung Above" | "Phandelver and Below: The Shattered Obelisk" | "Planescape: Adventures in the Multiverser" | "Players Handbook" | "Spelljammer: Adventures in Space" | "Sword Coast Adventurer's Guide" | "Strixhaven: A Curriculum of Chaos" | "Dragonlance: Shadow of the Dragon Queen" | "Tasha's Cauldron of Everything" | "Tyranny of Dragons" | "Volo's Guide to Monsters" | "The Wild Beyond the Witchlight" | "Wayfinder's Guide to Eberron" | "Xanathar's Guide to Everything";
```

# Abilities
```ts
type Abilities = "str" | "dex" | "con" | "int" | "wis" | "cha";
```

# Spell Level and Schools
```ts
type SpellLevels = 
  "cantrip" 
  | "1st" 
  | "2nd" 
  | "3rd" 
  | "4th" 
  | "5th" 
  | "6th" 
  | "7th" 
  | "8th" 
  | "9th";

type SpellSchools = 
  "abjuration" 
  | "conjuration" 
  | "divination" 
  | "enchantment" 
  | "evocation" 
  | "illusion" 
  | "necromancy" 
  | "transmutation";

type SpellCastTimes = 
  "action" 
  | "bonus action" 
  | "reaction" 
  | "min" 
  | "hr";

interface SpellRange {
  target: string,
  distance?: {
    amount: number,
    unit: string
  }
}
```

