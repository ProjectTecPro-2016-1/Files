## CLASS: ScoreScreen
	Description: Controls the player's score, the number of lines filled with boxes and  at the end of game shows all on screen.

### METHODS:
	```c++
	// -------------------------------------------------------------  
	// Function: ScoreScreen()  
	// Description: Constructor that loads image,socre font and score message for the Score Screen.
	// Return: void  
	// -------------------------------------------------------------  
	ScoreScreen() {
		...
	}
	```  
	
	```c++
	// -------------------------------------------------------------  
	// Function: ~ScoreScreen()  
	// Description: Destructor of class that cleans the "armario" surface, score message and score font.
	// Return: void  
	// -------------------------------------------------------------  
	~ScoreScreen() {
		...
	}
	```  
	
	```c++
	// -------------------------------------------------------------  
	// Function: drawSelf()  
	// Description: Applies score message, score font and "armario" image on screen to display the player's score. 
	// Parameters:
	//		SDL_Surface * surface;		Is the surface that the image will load.
	// Return: void  
	// -------------------------------------------------------------  
	void drawSelf(SDL_Surface * surface) {
		...
	}
	```  
	
	```c++
	// -------------------------------------------------------------  
	// Function: popLine()  
	// Description: Clean a line of boxes on screen when the player fills the line.
	// Return: void  
	// -------------------------------------------------------------  
	void popLine() {
		...
	}
	```  
	
	```c++
	// -------------------------------------------------------------  
	// Function: increaseScore()  
	// Description: Records the player's score on game.
	// Parameters:
	//		int value;		Value added on score for the final score. 
	// Return: void  
	// -------------------------------------------------------------  
	void increaseScore(int value) {
		...
	}
	```  
	
	```c++
	// -------------------------------------------------------------  
	// Function: lines()  
	// Description: Defines the number of rows that can be filled with boxes. 
	// Parameters: 
	//		int numero;		Number of lines that can be filled.
	// Return: void  
	// -------------------------------------------------------------  
	void lines(int numero) {
		...
	}
	```  
	
	```c++
	// -------------------------------------------------------------  
	// Function: scoring()  
	// Description: Writes the final value of the score on game.
	// Parameters:
	//		int value;		Value assigned the final score.	
	// Return: void  
	// -------------------------------------------------------------  
	void scoring(int value) {
		...
	}
	```  
	
	```c++
	// -------------------------------------------------------------  
	// Function: updateSelf()  
	// Description: Updates and shows on screen the score in the game and filled lines.
	// Return: void  
	// -------------------------------------------------------------  
	void updateSelf() {
		...
	}
	```  
	
	```c++
	// -------------------------------------------------------------  
	// Function: getLine()  
	// Description: Keeps a value of filled lines to display on screen at the end of game.
	// Return: int
	// -------------------------------------------------------------  
	int getLine() {
		...
	}
	```  
	
	```c++
	// -------------------------------------------------------------  
	// Function: getScorePoints()  
	// Description: Keeps the value of player's score at the end of game.
	// Return: int  
	// -------------------------------------------------------------  
	int getScorePoints() {
		...
	}
	```  
		
	```c++	
	// -------------------------------------------------------------  
	// Function: getBoxMessage()
	// Description: Return box message attribute
	// Return: SDL_Surface *
	// -------------------------------------------------------------  
	SDL_Surface * ScoreScreen::getBoxMessage() {
	    ...
	}
	```

	```c++
	// -------------------------------------------------------------  
	// Function: getgetArmario()
	// Description: Return armario attribute
	// Return: SDL_Surface *
	// -------------------------------------------------------------  
	SDL_Surface * ScoreScreen::getArmario() {
	    ...
	}
	```

	```c++
	// -------------------------------------------------------------  
	// Function: getScoreMessage()
	// Description: Return score message attribute
	// Return: SDL_Surface *
	// -------------------------------------------------------------  
	SDL_Surface * ScoreScreen::getScoreMessage() {
	    ...
	}
	```

	```c++
	// -------------------------------------------------------------  
	// Function: getScoreFont()
	// Description: Return score font attribute
	// Return: SDL_Surface *
	// -------------------------------------------------------------  
	TTF_Font * ScoreScreen::getScoreFont() {
	    ...
	}
	```

### ATTRIBUTES:
	```c++
	SDL_Surface * armario;			// Is a surface that contains all informataion about player's 
									// score at the end of game.
	TTF_Font * scoreFont;			// Is a font type loaded from a file, that can be used to shows the score. 
	SDL_Surface * scoreMessage;		// Is a surface that contains a "score message" which will be 
									// shown on screen. 
	SDL_Surface * boxMessage;		// Is the surface that contains a "box message" about the 
									// game at the time. 
	SDL_Color scoreTextColor;		// The color of "Score" which will be shown on the sreen.
	char scoreString[30];			// The value of score to be displayed on the screen.
	char lineString[30];			// The amount of line lefts to be displayed on the screen.
	int scorePoints;				// Real value of player's score. 
	int lineLeft;					// Real value of line lefts on game. 
	```  

### CONST:
	```c++
	static const int SCORE_WIDTH = 282;			// Size of width screen that will show the score, in pixels.
	static const int SCORE_HEIGHT = 456;		// Size of height screen that will show the score, in pixels.
	static const int SCORE_X_OFFSET = 506;		// Setpoint on the x axis where the score will be shown.
	static const int SCORE_Y_OFFSET = 10;		// Setpoint on the y axis where the score will be shown.
	```  
