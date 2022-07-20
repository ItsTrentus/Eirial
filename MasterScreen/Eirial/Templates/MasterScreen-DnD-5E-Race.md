## Type: template

## Icon: triton-head

## Creates: dnd 5e race

## Layout

|               |               |               |
| ------------- | ------------- | ------------- |
| Details       | Details       | Details       |
| DividerA      | DividerA      | DividerA      |
| Size          | Age           | Speed         |
| Traits        | Traits        | Traits        |
| Proficiencies | Proficiencies | Proficiencies |
| DividerB      | DividerB      | DividerB      |
| Defenses      | Resistances   | Immunities    |
| Names         | Names         | Names         |
| Effects       | Effects       | Effects       |


## Details
- type: text
- border
	- style: none

## Size
- type: text
- default: Medium
- text
	- align: center
- border
	- style: none

## Age
- type: number
- suffix: years
- text
	- align: center
- border
	- style: none

## Speed
- type: number
- suffix: ft
- text
	- align: center
- border
	- style: none

## Traits
- type: list
- of
	- type: text
- border
	- width: 3px
	- style: double

## Proficiencies
- type: set
- of
	- Armor
		- type: list
		- view: tags
		- of
			- type: text
	- Weapons
		- type: list
		- view: tags
		- of
			- type: text
	- Tools
		- type: list
		- view: tags
		- of
			- type: text
	- Languages
		- type: list
		- view: tags
		- of
			- type: text
	- Skills
		- type: list
		- view: tags
		- of
			- type: text
	- Saves
		- type: list
		- view: tags
		- of
			- type: text
- layout
	- 1
		
		|        |           |
		| ------ | --------- |
		| Armor  | Weapons   |
		| Tools  | Languages |
		| Skills | Saves     |
		
	- 500
		
		|           |         |       |
		| --------- | ------- | ----- |
		| Armor     | Weapons | Tools |
		| Languages | Skills  | Saves |
		
- text
	- align: center
- border
	- style: none

## Defenses
- type: list
- view: tags
- of
	- type: text
- text
	- align: center
- border
	- style: none

## Resistances
- type: list
- view: tags
- of
	- type: select
	- options
		1. Psychic
		2. Force
		3. Thunder
		4. Lightning
		5. Necrotic
		6. Radiant
		7. Cold
		8. Fire
		9. Acid
		10. Poison
		11. Bludgeoning
		12. Piercing
		13. Slashing
		14. Non-magic Bludgeoning
		15. Non-magic Piercing
		16. Non-magic Slashing
		17. Non-silvered Bludgeoning
		18. Non-silvered Piercing
		19. Non-silvered Slashing
- text
	- align: center
- border
	- style: none

## Immunities
- type: list
- view: tags
- of
	- type: select
	- options
		1. Psychic
		2. Force
		3. Thunder
		4. Lightning
		5. Necrotic
		6. Radiant
		7. Cold
		8. Fire
		9. Acid
		10. Poison
		11. Bludgeoning
		12. Piercing
		13. Slashing
		14. Non-magic Bludgeoning
		15. Non-magic Piercing
		16. Non-magic Slashing
		17. Non-silvered Bludgeoning
		18. Non-silvered Piercing
		19. Non-silvered Slashing
- text
	- align: center
- border
	- style: none

## Names
- type: text
- border
	- style: none

## Effects
- type: effects

## DividerA
- type: divider
- border
	- style: none

## DividerB
- type: divider
- border
	- style: none