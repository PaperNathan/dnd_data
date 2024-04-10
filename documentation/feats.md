# Feats
## Object Shapes
```ts
// Reference @/documentation/utility.md
interface Feat {
  name: string,
  abilityIncrease?: Record<Abilities + "choice", number>,
  prerequisite: string,
  source: SourceBooksAbbr
}