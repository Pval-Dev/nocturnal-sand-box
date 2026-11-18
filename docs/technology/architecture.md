# Technology and architecture

## Round orchestration

The server runs the round from lobby and voting through team selection, preparation, briefing, play, and results. It filters incompatible map and rule combinations, synchronizes phase timers, and clears round entities and restores terrain when the round ends.

## Server authority

The client handles input, camera, HUD, and presentation. The server validates requests and owns team membership, deployment, orders, objective state, damage, rewards, and persistent changes. Players receive the state needed for their current view and role.

## Combat and simulation

- Infantry coordinates movement, targeting, and distinct formation slots for each division.
- Tanks resolve hits against armor zones and impact angles and track ammunition and repairs.
- Aircraft combine distinct flight profiles with regional damage and flight state.
- Warships combine water navigation with regional damage, repairs, sinking, and boarding resolution.
- Objective rules use mode-specific entities and scoring, including convoy progress where supported.

## Persistence and presentation

Profile persistence covers loadouts, preferences, inventory, progression, and combat metrics. Match state and victory score belong to the current round. Dedicated PC and touch interfaces show the controls and instruments relevant to each mode.
