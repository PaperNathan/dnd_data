# Spells
## Object Shapes
```ts
// Reference @/documentation/utility.md
interface Spell {
  atHigherLevels: string,
  classes: string[],
  components: ("V" | "S" | "M")[],
  concentration: boolean,
  damage: string,
  damageType: string[],
  description: Entry[],
  duration: string,
  id: number,
  level: SpellLevels,
  materials?: string[],
  name: string,
  page: number,
  range: SpellRange,
  ritual: boolean,
  school: SpellSchools,
  source: SourceBooksAbbr,
  time: { number: number, unit: SpellCastTimes },
  upcast: string[]
}
```
# Example
```ts
const fireball: Spell = {
  atHigherLevels: "When you cast this spell using a spell slot of 4th level or higher, the damage increases by 1d6 for each slot level above 3rd.",
  components: ["V", "S", "M"],
  concentration: false,
  damage: "8d6",
  damageType: ["fire"],
  description: [
    {
      name: "Details",
      text: "A bright streak flashes from your pointing finger to a point you choose within range and then blossoms with a low roar into an explosion of flame. Each creature in a 20-foot-radius sphere centered on that point must make a Dexterity saving throw. A target takes 8d6 fire damage on a failed save, or half as much damage on a successful one."
    },
    {
      name: "Extra Information",
      text: "The fire spreads around corners. It ignites flammable objects in the area that aren't being worn or carried."
    }
  ],
  duration: "instant",
  id: "PHB241FB",
  level: "3rd",
  materials?: ["a tiny ball of bat guano", "sulfur"],
  name: "Fireball",
  page: 241,
  range: {
    target: "point",
    distance: {
      amount: 150,
      unit: "feet"
    }
  },
  ritual: false,
  school: "evocation",
  source: "PHB",
  time: { "number": 1, "unit": "action" },
  upcast: "1d6"
}
```
