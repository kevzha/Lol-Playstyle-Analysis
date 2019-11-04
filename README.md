# Lol-Playstyle-Analysis
Performed time-series clustering analysis to determine if there are common positional strategies in the game, League of Legends, divided by individual roles.

1. Obtained data through Riot's API for matches' timeline. Each timeline is obtained in a dictionary format where each event is given information such as frame(1 min intervals), event, timestamp, participants, and position.
2. Filtered the timeline dataframe for the desired events and positions of a player by roles. Some events might that did not contain positions were filtered out.
3. Calculate the distance between each event and the position of where I believe the player should be to have an impact on the team's chances of winning the match. The distance was calculated using the euclidean method.

<img src='map11.png' width="30%"/>
  The map is on a grid of x:14870, y:14980

4. Create a time series of the player distance from my understanding of their 'impactful' position throughout the the game.
5. Perform Hierarchical Agglomerative Clustering to group all the time series of a single role into similar positional locations throughout the game.
6. Display and interpret the resulting clusters(results shown below is for the top lane role)
   <br>Examples of interpretation: The first image shows that the player had a time period where they would stay in their top lane, but then swap to the other side of the map. This can be understood as the player destroying the top lane tower and swapped to the other side of the map in order to obtain the objective on that side of the map. Around the middle of the game, the player was focused on the middle of the map likely due to the team deciding to group together to push as a team towards the enemy base.

<img src='Resulting Clusters.png'/>
