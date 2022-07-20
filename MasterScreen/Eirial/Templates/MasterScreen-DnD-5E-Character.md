## Type: template

## Icon: barbute

## Creates: dnd 5e character

## Layout
- 1
	
	|               |               |               |
	| ------------- | ------------- | ------------- |
	| Armor Class   | Avatar        | Initiative    |
	| Level         | Avatar        | Proficiency   |
	| Experience    | Speed         | Inspiration   |
	| Stats         | Stats         | Stats         |
	| Hit Points    | Hit Points    | Hit Points    |
	| DividerA      | DividerA      | DividerA      |
	| Saves         | Saves         | Saves         |
	| Death Saves   | Death Saves   | Death Saves   |
	| Conditions    | Conditions    | Conditions    |
	| Features      | Features      | Features      |
	| Race          | Class         | Background    |
	| Subrace       | Subclass      | .             |
	| DividerB      | DividerB      | DividerB      |
	| Feats         | Defenses      | Senses        |
	| DividerC      | DividerC      | DividerC      |
	| Skills        | Skills        | Skills        |
	| Proficiencies | Proficiencies | Proficiencies |
	| Spellcasting  | Spellcasting  | Spellcasting  |
	| Items         | Items         | Items         |
	| Coins         | Coins         | Coins         |
	| DividerD      | DividerD      | DividerD      |
	| Appearance    | Appearance    | Appearance    |
	| Personality   | Personality   | Personality   |
	| Details       | Details       | Details       |
	
- 600
	
	|               |               |               |               |               |               |
	| ------------- | ------------- | ------------- | ------------- | ------------- | ------------- |
	| Avatar        | Level         | Proficiency   | Experience    | Speed         | Inspiration   |
	| Avatar        | Race          | Subrace       | Class         | Subclass      | Background    |
	| Stats         | Stats         | Stats         | Stats         | Stats         | Stats         |
	| Armor Class   | Hit Points    | Hit Points    | Hit Points    | Hit Points    | Initiative    |
	| DividerA      | DividerA      | DividerA      | DividerA      | DividerA      | DividerA      |
	| Saves         | Saves         | Conditions    | Conditions    | Death Saves   | Death Saves   |
	| Features      | Features      | Features      | Features      | Features      | Features      |
	| Feats         | Feats         | Defenses      | Defenses      | Senses        | Senses        |
	| DividerB      | DividerB      | DividerB      | DividerB      | DividerB      | DividerB      |
	| Skills        | Skills        | Skills        | Skills        | Skills        | Skills        |
	| Proficiencies | Proficiencies | Proficiencies | Proficiencies | Proficiencies | Proficiencies |
	| DividerC      | DividerC      | DividerC      | DividerC      | DividerC      | DividerC      |
	| Spellcasting  | Spellcasting  | Spellcasting  | Spellcasting  | Spellcasting  | Spellcasting  |
	| Items         | Items         | Items         | Items         | Items         | Items         |
	| Coins         | Coins         | Coins         | Coins         | Coins         | Coins         |
	| DividerD      | DividerD      | DividerD      | DividerD      | DividerD      | DividerD      |
	| Appearance    | Appearance    | Appearance    | Appearance    | Appearance    | Appearance    |
	| Personality   | Personality   | Personality   | Personality   | Personality   | Personality   |
	| Details       | Details       | Details       | Details       | Details       | Details       |
	

## Avatar
- type: image
- view: circle
- width: 120px
- height: 120px
- border
	- style: none
- untitled: yes

## Level
- type: select
- default: 1
- options
	1. 1
	2. 2
	3. 3
	4. 4
	5. 5
	6. 6
	7. 7
	8. 8
	9. 9
	10. 10
	11. 11
	12. 12
	13. 13
	14. 14
	15. 15
	16. 16
	17. 17
	18. 18
	19. 19
	20. 20
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

## Experience
- type: number
- suffix: xp
- default: 0
- text
	- align: center
- border
	- style: none

## Speed
- type: number
- suffix: ft
- default: 30
- text
	- align: center
- border
	- style: none

## Inspiration
- type: toggle
- icon: sun
- text
	- color: var(--color-yellow)
	- size: 1.4em
	- align: center
- border
	- style: none

## Race
- type: select
- text
	- align: center
- border
	- style: none
- effects: yes

## Subrace
- type: select
- text
	- align: center
- border
	- style: none
- effects: yes

## Class
- type: select
- text
	- align: center
- border
	- style: none
- effects: yes

## Subclass
- type: select
- text
	- align: center
- border
	- style: none
- effects: yes

## Background
- type: select
- effects: yes
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
	- color: var(--color-red)
- border
	- style: none

## Initiative
- type: number
- text
	- size: 1.4em
	- align: center

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
	- Bonus Actions
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
- border
	- style: none
- untitled: yes
- layout
	
	|               |
	| ------------- |
	| Abilities     |
	| Actions       |
	| Bonus Actions |
	| Reactions     |
	

## Feats
- type: list
- view: tags
- of
	- type: text
- text
	- align: center
- border
	- style: none
- effects: yes

## Defenses
- type: list
- view: tags
- of
	- type: text
- text
	- align: center
- border
	- style: none
- effects: yes

## Senses
- type: list
- view: tags
- of
	- type: text
- text
	- align: center
- border
	- style: none

## Skills
- type: set
- of
	- Deception
		- type: set
		- of
			- Proficient
				- type: toggle
				- view: circle
				- text
					- align: right
				- untitled: yes
			- Value
				- type: number
				- text
					- align: left
				- untitled: yes
		- layout
			
			|            |       |
			| ---------- | ----- |
			| Proficient | Value |
			
		- border
			- style: solid
	- Arcana
		- type: set
		- of
			- Proficient
				- type: toggle
				- view: circle
				- text
					- align: right
				- untitled: yes
			- Value
				- type: number
				- text
					- align: left
				- untitled: yes
		- layout
			
			|            |       |
			| ---------- | ----- |
			| Proficient | Value |
			
		- border
			- style: solid
	- Investigation
		- type: set
		- of
			- Proficient
				- type: toggle
				- view: circle
				- text
					- align: right
				- untitled: yes
			- Value
				- type: number
				- text
					- align: left
				- untitled: yes
		- layout
			
			|            |       |
			| ---------- | ----- |
			| Proficient | Value |
			
		- border
			- style: solid
	- Acrobatics
		- type: set
		- of
			- Proficient
				- type: toggle
				- view: circle
				- text
					- align: right
				- untitled: yes
			- Value
				- type: number
				- text
					- align: left
				- untitled: yes
		- layout
			
			|            |       |
			| ---------- | ----- |
			| Proficient | Value |
			
		- border
			- style: solid
	- Stealth
		- type: set
		- of
			- Proficient
				- type: toggle
				- view: circle
				- text
					- align: right
				- untitled: yes
			- Value
				- type: number
				- text
					- align: left
				- untitled: yes
		- layout
			
			|            |       |
			| ---------- | ----- |
			| Proficient | Value |
			
		- border
			- style: solid
	- Perception
		- type: set
		- of
			- Proficient
				- type: toggle
				- view: circle
				- text
					- align: right
				- untitled: yes
			- Value
				- type: number
				- text
					- align: left
				- untitled: yes
		- layout
			
			|            |       |
			| ---------- | ----- |
			| Proficient | Value |
			
		- border
			- style: solid
	- Nature
		- type: set
		- of
			- Proficient
				- type: toggle
				- view: circle
				- text
					- align: right
				- untitled: yes
			- Value
				- type: number
				- text
					- align: left
				- untitled: yes
		- layout
			
			|            |       |
			| ---------- | ----- |
			| Proficient | Value |
			
		- border
			- style: solid
	- Intimidation
		- type: set
		- of
			- Proficient
				- type: toggle
				- view: circle
				- text
					- align: right
				- untitled: yes
			- Value
				- type: number
				- text
					- align: left
				- untitled: yes
		- layout
			
			|            |       |
			| ---------- | ----- |
			| Proficient | Value |
			
		- border
			- style: solid
	- Animal Handling
		- type: set
		- of
			- Proficient
				- type: toggle
				- view: circle
				- text
					- align: right
				- untitled: yes
			- Value
				- type: number
				- text
					- align: left
				- untitled: yes
		- layout
			
			|            |       |
			| ---------- | ----- |
			| Proficient | Value |
			
		- border
			- style: solid
	- Sleight of Hand
		- type: set
		- of
			- Proficient
				- type: toggle
				- view: circle
				- text
					- align: right
				- untitled: yes
			- Value
				- type: number
				- text
					- align: left
				- untitled: yes
		- layout
			
			|            |       |
			| ---------- | ----- |
			| Proficient | Value |
			
		- border
			- style: solid
	- Performance
		- type: set
		- of
			- Proficient
				- type: toggle
				- view: circle
				- text
					- align: right
				- untitled: yes
			- Value
				- type: number
				- text
					- align: left
				- untitled: yes
		- layout
			
			|            |       |
			| ---------- | ----- |
			| Proficient | Value |
			
		- border
			- style: solid
	- Religion
		- type: set
		- of
			- Proficient
				- type: toggle
				- view: circle
				- text
					- align: right
				- untitled: yes
			- Value
				- type: number
				- text
					- align: left
				- untitled: yes
		- layout
			
			|            |       |
			| ---------- | ----- |
			| Proficient | Value |
			
		- border
			- style: solid
	- Athletics
		- type: set
		- of
			- Proficient
				- type: toggle
				- view: circle
				- text
					- align: right
				- untitled: yes
			- Value
				- type: number
				- text
					- align: left
				- untitled: yes
		- layout
			
			|            |       |
			| ---------- | ----- |
			| Proficient | Value |
			
		- border
			- style: solid
	- History
		- type: set
		- of
			- Proficient
				- type: toggle
				- view: circle
				- text
					- align: right
				- untitled: yes
			- Value
				- type: number
				- text
					- align: left
				- untitled: yes
		- layout
			
			|            |       |
			| ---------- | ----- |
			| Proficient | Value |
			
		- border
			- style: solid
	- Persuasion
		- type: set
		- of
			- Proficient
				- type: toggle
				- view: circle
				- text
					- align: right
				- untitled: yes
			- Value
				- type: number
				- text
					- align: left
				- untitled: yes
		- layout
			
			|            |       |
			| ---------- | ----- |
			| Proficient | Value |
			
		- border
			- style: solid
	- Insight
		- type: set
		- of
			- Proficient
				- type: toggle
				- view: circle
				- text
					- align: right
				- untitled: yes
			- Value
				- type: number
				- text
					- align: left
				- untitled: yes
		- layout
			
			|            |       |
			| ---------- | ----- |
			| Proficient | Value |
			
		- border
			- style: solid
	- Medicine
		- type: set
		- of
			- Proficient
				- type: toggle
				- view: circle
				- text
					- align: right
				- untitled: yes
			- Value
				- type: number
				- text
					- align: left
				- untitled: yes
		- layout
			
			|            |       |
			| ---------- | ----- |
			| Proficient | Value |
			
		- border
			- style: solid
	- Survival
		- type: set
		- of
			- Proficient
				- type: toggle
				- view: circle
				- text
					- align: right
				- untitled: yes
			- Value
				- type: number
				- text
					- align: left
				- untitled: yes
		- layout
			
			|            |       |
			| ---------- | ----- |
			| Proficient | Value |
			
		- border
			- style: solid
- border
	- style: none
- untitled: yes
- layout
	- 1
		
		|               |                 |
		| ------------- | --------------- |
		| Acrobatics    | Animal Handling |
		| Arcana        | Athletics       |
		| Deception     | History         |
		| Insight       | Intimidation    |
		| Investigation | Medicine        |
		| Nature        | Perception      |
		| Performance   | Persuasion      |
		| Religion      | Sleight of Hand |
		| Stealth       | Survival        |
		
	- 300
		
		|                 |                 |               |
		| --------------- | --------------- | ------------- |
		| Acrobatics      | Animal Handling | Arcana        |
		| Athletics       | Deception       | History       |
		| Insight         | Intimidation    | Investigation |
		| Medicine        | Nature          | Perception    |
		| Performance     | Persuasion      | Religion      |
		| Sleight of Hand | Stealth         | Survival      |
		
	- 600
		
		|             |                 |               |                 |           |            |
		| ----------- | --------------- | ------------- | --------------- | --------- | ---------- |
		| Acrobatics  | Animal Handling | Arcana        | Athletics       | Deception | History    |
		| Insight     | Intimidation    | Investigation | Medicine        | Nature    | Perception |
		| Performance | Persuasion      | Religion      | Sleight of Hand | Stealth   | Survival   |
		

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
- layout
	- 1
		
		|       |           |
		| ----- | --------- |
		| Armor | Weapons   |
		| Tools | Languages |
		
	- 600
		
		|       |         |       |           |
		| ----- | ------- | ----- | --------- |
		| Armor | Weapons | Tools | Languages |
		
- text
	- align: center
- border
	- style: none

## Spellcasting
- type: set
- of
	- Cantrips
		- type: number
		- text
			- align: center
			- size: 1.4em
	- Known
		- type: number
		- text
			- align: center
			- size: 1.4em
	- Modifier
		- type: number
		- text
			- align: center
	- Save
		- type: number
		- text
			- align: center
	- Attack
		- type: number
		- text
			- align: center
	- Slots
		- type: list
		- of
			- type: set
			- of
				- Level
					- type: number
					- default: 1
					- prefix: Level
					- untitled: yes
				- Slots
					- type: resource
					- default: 3/3
					- text
						- color: var(--color-blue)
					- untitled: yes
			- layout
				
				|       |       |       |       |       |
				| ----- | ----- | ----- | ----- | ----- |
				| Level | Slots | Slots | Slots | Slots |
				
	- Spells
		- type: items
		- view: table
		- show
			1. Level
			2. Duration
			3. Range
			4. Attack
- border
	- width: 3px
	- style: double
- layout
	
	|          |        |          |        |        |
	| -------- | ------ | -------- | ------ | ------ |
	| Cantrips | Known  | Modifier | Save   | Attack |
	| Slots    | Slots  | Slots    | Slots  | Slots  |
	| Spells   | Spells | Spells   | Spells | Spells |
	

## Items
- type: items
- effects: yes

## Coins
- type: set
- of
	- Copper
		- type: number
		- text
			- align: center
	- Silver
		- type: number
		- text
			- align: center
	- Electrum
		- type: number
		- text
			- align: center
	- Gold
		- type: number
		- text
			- align: center
	- Platinum
		- type: number
		- text
			- align: center
- border
	- style: none
- untitled: yes
- layout
	
	|        |        |          |      |          |
	| ------ | ------ | -------- | ---- | -------- |
	| Copper | Silver | Electrum | Gold | Platinum |
	

## Appearance
- type: set
- of
	- Age
		- type: number
		- default: 18
	- Eyes
		- type: text
	- Height
		- type: text
	- Skin
		- type: text
	- Hair
		- type: text
	- Weight
		- type: number
		- suffix: lbs
- layout
	- 1
		
		|      |      |        |
		| ---- | ---- | ------ |
		| Age  | Eyes | Height |
		| Skin | Hair | Weight |
		
	- 600
		
		|     |      |        |      |      |        |
		| --- | ---- | ------ | ---- | ---- | ------ |
		| Age | Eyes | Height | Skin | Hair | Weight |
		
- text
	- align: center

## Personality
- type: set
- of
	- Traits
		- type: text
		- text
			- align: center
	- Ideals
		- type: text
		- text
			- align: center
	- Bonds
		- type: text
		- text
			- align: center
	- Flaws
		- type: text
		- text
			- align: center
	- Alignment
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
	- Lifestyle
		- type: select
		- options
			1. Wretched
			2. Squalid (1SP)
			3. Poor (2SP)
			4. Modest (1GP)
			5. Comfortable (2GP)
			6. Wealthy (4GP)
			7. Aristocratic (10GP)
		- text
			- align: center
		- border
			- style: none
- border
	- style: none
- untitled: yes
- layout
	- 1
		
		|           |           |
		| --------- | --------- |
		| Traits    | Traits    |
		| Ideals    | Ideals    |
		| Bonds     | Bonds     |
		| Flaws     | Flaws     |
		| Alignment | Lifestyle |
		
	- 500
		
		|           |           |
		| --------- | --------- |
		| Traits    | Ideals    |
		| Bonds     | Flaws     |
		| Alignment | Lifestyle |
		

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

## DividerC
- type: divider
- border
	- style: none

## DividerD
- type: divider
- border
	- style: none