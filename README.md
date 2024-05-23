# Cart-pole-with-Q-learning-SARSA-and-Monte-carlo









![Untitled](https://github.com/mennatullahkransho/Cart-pole-with-Q-learning-SARSA-and-Monte-carlo/assets/120278669/00a520c4-a75a-4edf-8c40-69dc20458bc1)











Description
A pole is attached by an un-actuated joint to a cart, which moves
along a frictionless track. The pendulum starts upright, and the
goal is to prevent it from falling over by increasing and reducing
the cart&#39;s velocity.
 Source
This environment corresponds to the version of the cart-pole
problem described by Barto, Sutton, and Anderson

 Environment
o Observation
Type: Box (4)

Num Observation Min Max
0 Cart Position -2.4 2.4
1 Cart Velocity -Inf Inf
2 Pole Angle ~ -0.418 rad (-24°) ~ 0.418 rad (24°)
3 Pole Velocity At Tip -Inf Inf

o Actions
Type: Discrete (2)
Num Action
0 Push cart to the left
1 Push cart to the right

Note: The amount the velocity is reduced or increased is not fixed
as it depends on the angle the pole is pointing. This is because the
center of gravity of the pole increases the amount of energy
needed to move the cart underneath it

o Reward

Reward is 1 for every step taken, including the
termination step. The threshold is 475 for v1.
o Starting State
All observations are assigned a uniform random value
between ±0.05.
o Episode Termination
1. Pole Angle is more than ±12°
2. Cart Position is more than ±2.4 (center of the cart
reaches the edge of the display)
3. Episode length is greater than 200 (500 for v1).

 Solved Requirements
Considered solved when the average reward is greater than or
equal to 195.0 over 100 consecutive trials.
