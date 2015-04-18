# Battleship

<img src="http://i61.tinypic.com/6fumxc.png"></img>

Battleship is a javascript version of the popular game.
This javascript file will include a class for playing battleship. 
The main purpose is to see how fast a bot can clear the board in a specified amount of games.

Example of a sample bot / setting up a battleship game.
```javascript

	//Amount of games / size of board
	var b = new Battleship(100, 10);
	
	//amount of games to loop through
	for(var games = 0; games < b.amountOfGames; games++){
		
		//If the game isn't over continue to fire a random shot
		while(b.gameStatus.gameOver != true){
			b.fireShot(b.randomCoordinate());
		}
		
		//log the stats to the console.
		console.log(b.gameStats);
		
		//setup game
		b.drawBoard();
		b.createBoard();
		b.createShips();
		b.createGame();
		b.randomShipLocation(0);
		b.randomShipLocation(1);
		b.randomShipLocation(2);
		b.randomShipLocation(3);
		b.randomShipLocation(4);
	}
	//display the last game played
	b.drawStats();
```
