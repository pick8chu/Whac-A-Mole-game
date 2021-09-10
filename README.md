# Whac-A-Mole-game
## Requirements
1. score, time left, and start button are needed.
2. every hole(house) should be at least 50 x 50 big.
3. (\*) when a mole is out, it has to be displayed differently.
4. A round of game is 60 seconds long.
5. (\*) when refreshed, the game has to be remained
6. Maximum number of moles that are out is 5.
7. Duration of mole's out is from 1 second to 3.

## How I applied:
Only used vanilla js, no framework.

- made an array to manage status of all the buttons(holes/houses).
- used _setInterval_ function for timer.
- used session storage to maintain the current status of the game.
- each shot is considered as 100 points.
- randomizing the show-up time, and when to show up were little tricky. I made it to run function _randomButtonOn_ 3 times in every seconds, and in _randomButtonOn_ it has _doable_ function which decides if it's a good time to make a mole show up. On every execution of _randomButtonOn_, there are 60% chances of false which would not let mole out. So with 40% of chance and when there are less than 5 moles out, it would let any mole out for 1~3 seconds.
