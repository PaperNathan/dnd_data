# Items
## Armor
```ts
// Reference @/documentation/utility.md
interface Armor {
  ac: number,
  bonusAC: Abilities | number,
  cursed: boolean,
  description: Entry[]
  name: string,
  page: number,
  rarity: string,
  source: SourceBooksAbbr,
  type: string,
  value: number,
  weight: number,
}
```

## Weapons
```ts
// Reference @/documentation/utility.md
interface Weapon {
  category: "simple" | "martial",
  characterModifier: CharacterModifier[]
  cursed: boolean,
  damage: string[],
  damageType: string[],
  description: Entry[]
  name: string,
  page: number,
  properties: string[],
  range: string,
  rarity: string,
  source: SourceBooksAbbr,
  type: string,
  value: number,
  weight: number,
}
```

### Weapon Example
```ts
const weapon: Weapon = {
  category: "martial",
  characterModifier: [
    dex: "modifier",
    modifier: 2
  ],
  cursed: true,
  damage: "2d6",
  damageType: "slashing",
  description: [
    {
      name: "Agile Slasher",
      text: "This weapon is easy to wield.  While wielding this weapon you gain a +2 bonus to your Dexterity (DEX)."
    },
    {
      name: "Curse: Hard to Put Down",
      text: "This sword can not leave your hand.  If left unattended for 1d4 days, it will fuse and become your hand.  If it becomes your hand, you have disadvantage on Sleight of Hand checks."
    }
  ]
  name: "Speedy Greatsword",
  page: 149,
  properties: [
    "2-handed"
  ],
  range: 5,
  rarity: "none",
  source: "PHB",
  type: "sword",
  value: 50000,
  weight: 2,
}
```

## Other
```ts
interface Item {

}
```