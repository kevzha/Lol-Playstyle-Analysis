# Lol-Playstyle-Analysis
Performed time-series clustering analysis to see if there is a common strategies in the game League of Legends divided per role

1. Obtained data through Riot's API for a matches' timeline, which includes events, timestamps and positions on the map the player is.
2. Filter the timeline for useful events and positions of a player by roles
3. Calculate the distance between each event and the position of where the player should be to have the most impact.

<img src='map11.png' width="30%"/>
  The map is on a grid of x:14870, y:14980

4. Create the time series of the player distance throughout the duration of the game.
5. Perform HAC to perform clustering analysis on all the time series of a single role.
6. Interpret the resulting clusters:

<img src='Resulting Clusters.png'/>


