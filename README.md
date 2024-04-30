**Unit production from barracks:**

-	The changes in Lasyabot.java are significantly based on the BasicRush Implementation by Damon.
-	My changes mainly are about the unit production from barracks, particularly focusing on ranged units.
- Initially there was no specific logic for producing ranged units in waves or groups , so i tried to introduce a wave-based production strategy for ranged units(Where i took units 4 and 3).
- Ranged units are produced in alternating waves of 4 and 3 units, depending on the available resources and a counter that tracks the number of waves produced.
- This strategy is encapsulated within the Barracks class's assignTask method.
- This change aims to optimize resource use and enhance strategic deployment of ranged units.

**Unit Production:**
- Initially the decision to train units was more straightforward and did not consider grouping units into waves.
- So i tried checking if the resources are sufficient to produce an entire wave of ranged units (either 4 or 3 depending on the cycle).
- If resources are not enough for a wave, it falls back to producing lighter units if resources permit.

**To Summarize my changes**
- I tried to introduce a strategy where the bot creates groups of ranged units in a more organized way.
- This approach helps the bot deploy units at the right time, which can be really useful in different game situations.
- By managing resources and timing better, this new method could make the bot more effective at attacking or defending, ultimately improving how it performs in the game.
