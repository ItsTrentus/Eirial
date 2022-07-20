## Type: template

## Icon: crossed-sabres

## Creates: dnd 5e class

## Layout

|               |               |               |
| ------------- | ------------- | ------------- |
| Details       | Details       | Details       |
| Class Table   | Class Table   | Class Table   |
| Hit Points    | Hit Points    | Hit Points    |
| Features      | Features      | Features      |
| Proficiencies | Proficiencies | Proficiencies |
| Spellcasting  | Spellcasting  | Spellcasting  |
| Equipment     | Equipment     | Equipment     |
| Effects       | Effects       | Effects       |


## Details
- type: text
- border
	- style: none

## Class Table
- type: table

## Hit Points
- type: set
- of
	- Hit Dice
		- type: text
	- First Level
		- type: text
	- Higher Levels
		- type: text
- text
	- align: center
- border
	- style: none
- layout
	- 1
		
		|               |
		| ------------- |
		| Hit Dice      |
		| First Level   |
		| Higher Levels |
		
	- 500
		
		|          |             |               |
		| -------- | ----------- | ------------- |
		| Hit Dice | First Level | Higher Levels |
		

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

## Spellcasting
- type: set
- of
	- Cantrips
		- type: text
		- text
			- align: center
	- Slots
		- type: text
		- text
			- align: center
	- Known
		- type: text
		- text
			- align: center
	- Modifier
		- type: text
		- text
			- align: center
	- Save
		- type: text
		- text
			- align: center
	- Attack
		- type: text
		- text
			- align: center
	- Details
		- type: text
- layout
	- 1
		
		|          |          |
		| -------- | -------- |
		| Cantrips | Slots    |
		| Known    | Modifier |
		| Save     | Attack   |
		| Details  | Details  |
		
	- 500
		
		|          |         |         |
		| -------- | ------- | ------- |
		| Cantrips | Slots   | Known   |
		| Modifier | Save    | Attack  |
		| Details  | Details | Details |
		

## Equipment
- type: list
- view: tags
- of
	- type: text
- text
	- align: center
- border
	- style: none

## Effects
- type: effects