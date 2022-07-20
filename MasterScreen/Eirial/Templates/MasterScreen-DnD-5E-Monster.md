## Type: template

## Icon: sharp-smile

## Creates: dnd 5e monster

## Layout
- 1
	
	|             |             |             |
	| ----------- | ----------- | ----------- |
	| Armor Class | Armor Class | Armor Class |
	| Challenge   | Speed       | Proficiency |
	| Stats       | Stats       | Stats       |
	| Hit Points  | Hit Points  | Hit Points  |
	| DividerA    | DividerA    | DividerA    |
	| Saves       | Saves       | Saves       |
	| Death Saves | Death Saves | Death Saves |
	| Conditions  | Conditions  | Conditions  |
	| Features    | Features    | Features    |
	| Reward      | Species     | Alignment   |
	| DividerB    | DividerB    | DividerB    |
	| Languages   | Skills      | Senses      |
	| Immunities  | Defenses    | .           |
	| Details     | Details     | Details     |
	
- 600
	
	|             |             |            |            |             |             |
	| ----------- | ----------- | ---------- | ---------- | ----------- | ----------- |
	| Challenge   | Proficiency | Species    | Reward     | Speed       | Alignment   |
	| Stats       | Stats       | Stats      | Stats      | Stats       | Stats       |
	| Armor Class | Hit Points  | Hit Points | Hit Points | Hit Points  | .           |
	| DividerA    | DividerA    | DividerA   | DividerA   | DividerA    | DividerA    |
	| Saves       | Saves       | Conditions | Conditions | Death Saves | Death Saves |
	| Features    | Features    | Features   | Features   | Features    | Features    |
	| Skills      | Skills      | Languages  | Languages  | Senses      | Senses      |
	| Defenses    | Defenses    | Immunities | Immunities | .           | .           |
	| DividerB    | DividerB    | DividerB   | DividerB   | DividerB    | DividerB    |
	| Details     | Details     | Details    | Details    | Details     | Details     |
	

## Challenge
- type: number
- text
	- align: center
- border
	- style: none

## Proficiency
- type: select
- prefix: +
- default: 2
- options
	1. 2
	2. 3
	3. 4
	4. 5
	5. 6
- border
	- style: none

## Species
- type: text
- text
	- align: center
- border
	- style: none

## Reward
- type: number
- suffix: xp
- text
	- align: center
- border
	- style: none

## Speed
- type: number
- text
	- align: center
- border
	- style: none
- suffix: ft

## Alignment
- type: select
- options
	1. Lawful Good
	2. Neutral Good
	3. Chaotic Good
	4. Lawful Neutral
	5. True Neutral
	6. Chaotic Neutral
	7. Lawful Evil
	8. Neutral Evil
	9. Chaotic Evil
- text
	- align: center
- border
	- style: none

## Stats
- type: set
- of
	- Strength
		- type: number
		- default: 10
	- Dexterity
		- type: number
		- default: 10
	- Constitution
		- type: number
		- default: 10
	- Intelligence
		- type: number
		- default: 10
	- Wisdom
		- type: number
		- default: 10
	- Charisma
		- type: number
		- default: 10
- layout
	- 1
		
		|              |           |              |
		| ------------ | --------- | ------------ |
		| Strength     | Dexterity | Constitution |
		| Intelligence | Wisdom    | Charisma     |
		
	- 500
		
		|          |           |              |              |        |          |
		| -------- | --------- | ------------ | ------------ | ------ | -------- |
		| Strength | Dexterity | Constitution | Intelligence | Wisdom | Charisma |
		
- text
	- size: 1.4em
	- align: center
- border
	- width: 3px
	- style: double
- untitled: yes

## Armor Class
- type: number
- text
	- size: 1.4em
	- align: center

## Hit Points
- type: resource
- text
	- color: purple
- border
	- style: none

## Saves
- type: set
- of
	- Strength
		- type: text
	- Dexterity
		- type: text
	- Constitution
		- type: text
	- Intelligence
		- type: text
	- Wisdom
		- type: text
	- Charisma
		- type: text
- layout
	
	|              |           |              |
	| ------------ | --------- | ------------ |
	| Strength     | Dexterity | Constitution |
	| Intelligence | Wisdom    | Charisma     |
	
- text
	- align: center
- border
	- style: none

## Conditions
- type: list
- view: tags
- of
	- type: select
	- options
		1. Blinded
		2. Charmed
		3. Deafened
		4. Frightened
		5. Grappled
		6. Incapacitated
		7. Invisible
		8. Paralyzed
		9. Petrified
		10. Poisoned
		11. Prone
		12. Restrained
		13. Stunned
		14. Unconscious
		15. Exhaustion
- text
	- align: center
- border
	- style: none
- effects: yes

## Death Saves
- type: set
- of
	- Save
		- type: resource
		- view: points
		- icon: vine-leaf
		- default: 0/3
		- text
			- color: var(--color-green)
		- untitled: yes
	- Fail
		- type: resource
		- view: points
		- icon: death-skull
		- default: 0/3
		- text
			- color: var(--color-red)
		- untitled: yes
- layout
	
	|      |
	| ---- |
	| Save |
	| Fail |
	
- text
	- size: 1.4em
- border
	- style: none

## Features
- type: set
- view: tabs
- of
	- Abilities
		- type: list
		- of
			- type: set
			- of
				- Details
					- type: text
					- untitled: yes
				- Uses
					- type: resource
					- view: points
					- default: 1/1
					- untitled: yes
			- layout
				
				|         |         |         |         |         |         |         |         |      |
				| ------- | ------- | ------- | ------- | ------- | ------- | ------- | ------- | ---- |
				| Details | Details | Details | Details | Details | Details | Details | Details | Uses |
				
		- border
			- style: solid
	- Actions
		- type: list
		- of
			- type: set
			- of
				- Details
					- type: text
					- untitled: yes
				- Uses
					- type: resource
					- view: points
					- default: 1/1
					- untitled: yes
			- layout
				
				|         |         |         |         |         |         |         |         |      |
				| ------- | ------- | ------- | ------- | ------- | ------- | ------- | ------- | ---- |
				| Details | Details | Details | Details | Details | Details | Details | Details | Uses |
				
		- border
			- style: solid
	- Reactions
		- type: list
		- of
			- type: set
			- of
				- Details
					- type: text
					- untitled: yes
				- Uses
					- type: resource
					- view: points
					- default: 1/1
					- untitled: yes
			- layout
				
				|         |         |         |         |         |         |         |         |      |
				| ------- | ------- | ------- | ------- | ------- | ------- | ------- | ------- | ---- |
				| Details | Details | Details | Details | Details | Details | Details | Details | Uses |
				
		- border
			- style: solid
	- Legendary Actions
		- type: list
		- of
			- type: set
			- of
				- Details
					- type: text
					- untitled: yes
				- Uses
					- type: resource
					- view: points
					- default: 1/1
					- untitled: yes
			- layout
				
				|         |         |         |         |         |         |         |         |      |
				| ------- | ------- | ------- | ------- | ------- | ------- | ------- | ------- | ---- |
				| Details | Details | Details | Details | Details | Details | Details | Details | Uses |
				
		- border
			- style: solid
- border
	- style: none
- untitled: yes
- layout
	
	|                   |
	| ----------------- |
	| Abilities         |
	| Actions           |
	| Reactions         |
	| Legendary Actions |
	

## Skills
- type: list
- of
	- type: text
- view: tags
- text
	- align: center
- border
	- style: none

## Senses
- type: list
- of
	- type: text
- view: tags
- text
	- align: center
- border
	- style: none

## Languages
- type: list
- of
	- type: text
- view: tags
- text
	- align: center
- border
	- style: none

## Defenses
- type: list
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
- view: tags
- text
	- align: center
- border
	- style: none

## Immunities
- type: list
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
		20. Blinded
		21. Charmed
		22. Deafened
		23. Frightened
		24. Grappled
		25. Incapacitated
		26. Invisible
		27. Paralyzed
		28. Petrified
		29. Poisoned
		30. Prone
		31. Restrained
		32. Stunned
		33. Unconscious
		34. Exhaustion
- view: tags
- text
	- align: center
- border
	- style: none

## Details
- type: text
- border
	- style: none

## DividerA
- type: divider
- border
	- style: none

## DividerB
- type: divider
- border
	- style: none