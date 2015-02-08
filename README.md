# Battleship

Battleship is a javascript version of the popular game.
This javascript file will include an api for building a bot. 
The main purpose is to see how fast a bot can clear the board in a specified amount of games.

Example of a sample bot / setting up a battlship game.
'''
	var b = new Battleship(100, 10);
	for(var games = 0; games < b.amountOfGames; games++){
		while(b.gameStatus.gameOver != true){
			b.fireShot(b.randomCoordinate());
		}
		console.log(b.gameStats);
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
	b.drawStats();
'''
