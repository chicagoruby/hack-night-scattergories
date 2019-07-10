# Scattergories

Scattergories is a timed word game that requires you to think quickly in order to name responses that fit a list of given categories that all begin with a randomly selected letter. The classic party game pits up to 6 players against eachother, each with the same list of categories and the same beginning letter. The player with the most accepted words filled out within the given time frame wins that round.

## Gameplay

For each round, players are given a list of 12 categories. A category would be something like "a boy's name" or "things you find in a desk drawer". A 20 sided dice is rolled to determine the beginning letter that each of the responses must start with. The dice sides are all letters with the exception of Q, U, V, X, Y, and Z. Once the dice is rolled, a 3 minute timer is set and the players begin to fill out their responses.

Each response must begin with the letter that is displayed on the dice. For example, if the letter drawn is "J", a response to "a boys name" may be "Steve", and a response to "things you find in a desk drawer" may be "staples". While only one response per category can be accepted, alliteration is encouraged and counts for extra points when used. For example, if the category is "fictional characters" and the letter is "B", then "Bugs Bunny" would be worth 2 points for that category.

When the timer finishes, then players may no longer add or edit responses. In the multi-player version, answers are read for each player for each category. If more than one player has written the same response, than neither earns a point, so the more unique the responses, the more likely it will be rewarded with a point.

## The Application

Your app should be playable in single player or multiple player mode.

### Single Player Mode

Begin with a single player version of the game that assigns categories from the JSON list provided in the repo for each round. There are a total of 16 rounds and no category should be repeated across rounds.

Set a timer and display the categories. Allow the user to input responses for each category. When the timer goes off, count the number of responses.

What feedback will be given to the user? How will you know when an answer is valid (ie: "taco" would not be an acceptable answer for a "country" that begins with the letter "T") and should be counted? How will you account for multi-point answers?

### Multi-Player Mode

Allow multiple players to play with the same category list. You can accomplish this in a couple of different ways. You can implement a networked solution that allows users on different machines to work with the same list and letter. A more basic solution would be to have the players play in succession, one at a time, with the previous player's answers hidden.

The score calculation for multiple players will have to account for possible response duplication. Remember, if two players have the same response, neither gets a point.

The player with the most points at the end of the round wins that round. Keep track of the players scores during a session and allow them to play multiple rounds to determine an overall champion.
