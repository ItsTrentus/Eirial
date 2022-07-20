## Type: template

## Icon: burning-dot

## Creates: dnd 5e spell

## Layout
- 1
	
	|               |             |
	| ------------- | ----------- |
	| Level         | School      |
	| Cast          | Duration    |
	| DividerA      | DividerA    |
	| Details       | Details     |
	| Components    | Range       |
	| Attack        | Damage      |
	| Concentration | Ritual      |
	
- 700
	
	|            |           |           |               |           |
	| ---------- | --------- | --------- | ------------- | --------- |
	| Level      | School    | Cast      | Duration      | Range     |
	| Components | Attack    | Damage    | Concentration | Ritual    |
	| DividerA   | DividerA  | DividerA  | DividerA      | DividerA  |
	| Details    | Details   | Details   | Details       | Details   |
	| Details    | Details   | Details   | Details       | Details   |
	

## Level
- type: select
- default: 0
- options
	1. 0
	2. 1
	3. 2
	4. 3
	5. 4
	6. 5
	7. 6
	8. 7
	9. 8
	10. 9
- border
	- style: none

## School
- type: select
- default: Abjuration
- options
	1. Abjuration
	2. Conjuration
	3. Divination
	4. Enchantment
	5. Evocation
	6. Illusion
	7. Necromancy
	8. Transmutation
- border
	- style: none

## Cast
- type: select
- default: 1 Action
- options
	1. 1 Action
	2. 1 Bonus action
	3. 1 Reaction
	4. 1 Minute
	5. 10 Minutes
	6. 1 Hour
	7. 8 Hours
	8. 12 Hours
	9. 24 Hours
- border
	- style: none

## Duration
- type: select
- default: Instantaneous
- options
	1. Instantaneous
	2. 1 Round
	3. 1 Minute
	4. 10 Minutes
	5. 1 Hour
	6. 8 Hours
	7. 12 Hours
	8. 24 Hours
	9. 1 Day
	10. 7 days
	11. 10 days
	12. Until Dispelled
- border
	- style: none

## Range
- type: text
- text
	- align: center
- border
	- style: none

## Components
- type: text
- text
	- align: center
- border
	- style: none

## Attack
- type: text
- text
	- align: center
- border
	- style: none

## Damage
- type: text
- text
	- align: center
- border
	- style: none

## Concentration
- type: toggle
- view: circle
- text
	- align: center
- border
	- style: none

## Ritual
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

## DividerA
- type: divider
- border
	- style: none