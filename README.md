# BGG Data Fetcher

This script will fetch board games data from BoardGameGeek API and store the data in a CSV file. The API response is in XML format and since there is no endpoint in order to fetch multiple board games data at once, this will work by making a request to the endpoint for a single board game based on board game(s) ID, while incrementing the ID after each request withing the given range of IDs.

The information fetched and stored for each board game is the following:

`name`, `game_id`, `rating`, `weight`, `year_published`, `min_players`, `max_players`, `min_play_time`, `max_pay_time`, `min_age`, `owned_by`, `categories`, `mechanics`, `designers`, `artists` and `publishers`.
