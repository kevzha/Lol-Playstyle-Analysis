# Lol-Playstyle-Analysis
Performed time-series clustering analysis to see if there is a common strategies in the game League of Legends divided per role

1. Obtained data through Riot's API for a matches' timeline, which includes events, timestamps and positions on the map the player is.
2. Filter the timeline for useful events and positions of a player by roles
3. Calculate the distance between each event and the position of where the player should be to have the most impact.
4. Create the time series of the player distance throughout the duration of the game.
