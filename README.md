# rpg-idea
turn based rpg ideas

## stats description

- mental:
  -- fortitude:
  -- endurance:
  -- dexterity:
  -- agility:

- physical:
  -- fortitude:
  -- endurance:
  -- dexterity:
  -- agility:

## battle description

- Combos:
 As your character levels your character will gain combo recipes. Each recipe will have an effect which applies on the enemy. A combo can be executed in one turn, the length of the combo will affect the accuracy of each attack/spell node; however, your character level and dexterity(mental and physical) can counteract the effect. A combo can be spell and/or attack chains.

- Attack chains:
 Each attack will have a place in a graph, if the attack has linking attributes to another if will add multiplier on the effects of the next attack depending on the level of the initial attacking character, the multiplier will decrease according to the attack's distance to the next one on the graph:
 -- e.g.: Alpha attacks, next Beta attacks, the computation will be Beta's attack total = attackStrength * levelMultiplier + attackStrength * (Alpha's level * multiplier(numberOfNodes/(10^digits)))
 -- so: 150 * (3 ln(3)) + 3 * (2/10), or 1200 * (100 ln(100)) + 100 * (12/100)

- defense chains:
 This will replicate the attack computation but with defense characteristics

- battle length:
 If the battle lasts too long, the enemy or the character may suffer exhaustion effects which may increase your winning or losing chances

- exhaustion effects:
 Depending on the character stats this will have effects on either your Stamina or Mana. Both are descriptors for Mental endurance or physical.
 -- e.g.: as you deplete your Mana your spells become less accurate and less potent, if you consume most of your Mana on a single spell(possible) the spell will be fine, but if you're on your 20th cast in the battle, the accuracy will be reduced according to (ManaAmount * 1/characterLevel)/ManaAmount, so (100 * 1/10)/100, which results in a 10% reduction to accuracy.


## Leveling description

As your character levels up certain characteristics will be addressed:
- Combos - the more your character uses a set of combos the higher the efficiency(less cost on stamina/Mana), however the less often you use them, the more a punitive affect will be applied on the combo's efficacy.
- Spells - spells may actually fade from your character's memory if they become disused. I'm trying to replicate the mind and its reaction to garbage cleaning. The more a spell is used the less Mana it will cost.
- Attacks will have the same affect as above.
- Refreshers, if your character loses focus of a spell/attack, you can ingest refreshers and select the spell/attack to refresh the focus.
- Your character may actually completely lose an attack/spell if it goes disused long enough. You'll have to relearn it through Teachers.

### Teachers

Your character will meet teachers, which will be marked post hoc, who will teach your character spells/attacks.
