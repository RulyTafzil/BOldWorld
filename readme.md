# Introduction
A mod for the game Old World to improve combat and early game aggression.

# Improved Damage Calculation
Vanilla Old World calculates damage as $$\frac{\text{Attacker's Attack}}{\text{Defender's Defense}} \cdot 6 = \text{Damage Rounded to Integer in Favor of Stronger Unit}$$ 

This results in many unintutive outcomes, especially in regards to small percentage bonuses such as the 5/10/15% bonsues from the "Combat I/II/III" unit upgrades, or the 10% bonuse from units in their home territory. 

For example, consider a Warrior (Strength 4) attacking a Spearman (Strength 5), where the Warrior gains a 5% or 10% bonus.

$\frac{4}{5} \cdot 6 = 4.8$ Rounds to 4

$\frac{4.2}{5} \cdot 6 = 5.04$ Rounds to 5

$\frac{4.4}{5} \cdot 6 = 5.28$ Rounds to 5

Without any bonuses the damage is 4.8 rounded down to 4 in favor of the Spearman. With a 5% buff, the Warrior's attack strength becomes 4.2 and results in 5.04 damage, rounded down to 5. This results in an effective 25% damage increase. Far more than the 5% expected. With a 10% buff the Warrior's attack becomes 4.4, raising the calucated damage to 5.28. However, this still rounds down to 5, resulting in effectivley no difference from the 5% buffed warrior. 


This mod raises HP and Damage values of everything by a favor of 5. This allows smaaller percentage bonuses to be accurately reflected and minimizes the unintutive effect of rounding damage. 

Using the examples above of a Warrior vs a Spearmen at base, 5% and 10% bonuses, we now get damage values of:

$\frac{4}{5} \cdot 30 = 24$ Rounds to 24

$\frac{4.2}{5} \cdot 30 = 25.2$ Rounds to 25

$\frac{4.4}{5} \cdot 30 = 26.4$ Rounds to 26
