## Type: template

## Icon: ring

## Creates: dnd 5e item

## Layout
- 1
	
	|             |             |
	| ----------- | ----------- |
	| Item Type   | Rarity      |
	| Price       | Attunement  |
	| DividerA    | DividerA    |
	| Details     | Details     |
	| Effects     | Effects     |
	
- 500
	
	|             |             |             |             |
	| ----------- | ----------- | ----------- | ----------- |
	| Item Type   | Rarity      | Price       | Attunement  |
	| DividerA    | DividerA    | DividerA    | DividerA    |
	| Details     | Details     | Details     | Details     |
	| Effects     | Effects     | Effects     | Effects     |
	

## Item Type
- type: select
- default: Item
- options
	1. Armor
	2. Artifact
	3. Item
	4. Potion
	5. Ring
	6. Rod
	7. Scroll
	8. Staff
	9. Wand
	10. Weapon
	11. Wondrous
	12. Other
- border
	- style: none

## Rarity
- type: select
- default: Common
- options
	1. Common
	2. Uncommon
	3. Rare
	4. Very rare
	5. Legendary
	6. Sentient
- border
	- style: none

## Price
- type: number
- suffix: Gold
- text
	- align: center
- border
	- style: none

## Attunement
- type: toggle
- view: circle
- text
	- align: center
- border
	- style: none

## Details
- type: text
- border
	- style: none

## Effects
- type: effects

## DividerA
- type: divider
- border
	- style: none