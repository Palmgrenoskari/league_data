# league_data
Figuring out how to extract all the necessary data for my league analytics page from League of legends API.

**Update: The current API call limit of 100 requests / 2 min is too small for getting reasonable aggregate data from match histories.**

**I'm applying for a Dev API key very soon.**

The available method for getting match data is the following:

Start from 1-5 player ids, pull their match histories, grab the player ids of the other players in the matches, pull those match histories, repeat

It becomes even more "request heavy" if you want to include player ranks in the mix since you need to pull ranks from another endpoint for each player and then call yet another endpoint to match the summoner id with player id.
