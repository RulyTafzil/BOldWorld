# Introduction
A mod for the game Old World to improve combat and early game aggression.

# Improved Damage Calculation
Vanilla Old World calculates damage as:
$$\frac{\text{Attacker's Attack}}{\text{Defender's Defense}} \cdot 6 = \text{Damage}$$ 
Where the value is rounded to an integer in favor of the stronger unit. This can result in many unintutive outcomes, especially in regards to small percentage bonuses that can come from unit upgrades or family bonuses. 

For example, consider a Warrior (Strength 4) attacking a Spearman (Strength 5). Without any bonuses the damage is calculated as:

$\frac{4}{5} \cdot 6 = 4.8$ As the Spearman is stronger, this gets rounded down to 4. 

With a 5% buff, the Warrior's attack strength becomes 4.2. However, as seen below, this causes the damage to break above 5, resulting in an effective 25% damage increase. 

$\frac{4.2}{5} \cdot 6 = 5.04$ As the Spearman is stronger, this gets rounded down to 5. 

With a 10% buff, the Warrior's attack becomes 4.4, raising the calucated damage to 5.28, which still rounds to 5, resulting in effectivley no difference from the 5% buffed warrior. 
$\frac{4.4}{5} \cdot 6 = 5.28$ As the Spearman is stronger, this gets rounded down to 4. 
