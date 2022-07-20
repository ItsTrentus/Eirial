## Type: template

## Icon: book-cover

## Creates: dnd 5e background

## Layout
- 100
	
	|               |
	|---------------|
	| Details       |
	| Features      |
	| Proficiencies |
	| DividerA      |
	| Equipment     |
	| Personality   |
	| Effects       |
	
- 500
	
	|               |               |               |               |
	| ------------- | ------------- | ------------- | ------------- |
	| Details       | Details       | Details       | Details       |
	| Features      | Features      | Features      | Features      |
	| Proficiencies | Proficiencies | Proficiencies | Proficiencies |
	| DividerA      | DividerA      | DividerA      | DividerA      |
	| Equipment     | Equipment     | Equipment     | Equipment     |
	| Personality   | Personality   | Personality   | Personality   |
	| Effects       | Effects       | Effects       | Effects       |
	

## Details
- type: text
- border
	- style: none

## Features
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
		|--------|-----------|
		| Armor  | Weapons   |
		| Tools  | Languages |
		| Skills | Saves     |
		
	- 500
		
		|           |         |       |
		|-----------|---------|-------|
		| Armor     | Weapons | Tools |
		| Languages | Skills  | Saves |
		
- text
	- align: center
- border
	- style: none

## Equipment
- type: list
- view: tags
- of
	- type: text
- text
	- align: center
- border
	- style: none

## Personality
- type: set
- of
	- Traits
		- type: list
		- of
			- type: text
		- border
			- style: none
	- Ideals
		- type: list
		- of
			- type: text
		- border
			- style: none
	- Bonds
		- type: list
		- of
			- type: text
		- border
			- style: none
	- Flaws
		- type: list
		- of
			- type: text
		- border
			- style: none

## Effects
- type: effects

## DividerA
- type: divider
- border
	- style: none