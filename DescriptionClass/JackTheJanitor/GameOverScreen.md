## CLASS: GameOverScreen
	Description: Controls all actions that the screen runs at the end of the game.

### METHODS:
	```c++
	// -------------------------------------------------------------  
	// Function: GameOverScreen()  
	// Description: Load the image of level on screen.
	// Parameters:
	//		string filename;		Name of a image file of level that will be showed on screen.
	// Return: void  
	// -------------------------------------------------------------  
	GameOverScreen(std::string filename) {
		...
	}
	```  
	
	```c++
	// -------------------------------------------------------------  
	// Function: ~GameOverScreen()  
	// Description: Destructor of class that clean the screen.
	// Return: void  
	// -------------------------------------------------------------  
    ~GameOverScreen() {
		...
	}
	```  
	
	```c++
	// -------------------------------------------------------------  
	// Function: drawSelf()  
	// Description: Draws the image on screen, according to the level.
	// Parameters:
	//		SDL_Surface * surface;		Is the surface that the image will load.
	// Attributes: nothing
	// Return: void  
	// -------------------------------------------------------------  
	void drawSelf(SDL_Surface *surface) {
		...
	}
	```  

### ATRIBUTTES:
	```c++
	SDL_Surface *gameOverScreen;		// Keeps the image that loaded.
	```  
	
### CONST:
	```c++
	static const int LEVEL_WIDTH = 854;			// Size of width screen that will show the image level, in pixels.
    static const int LEVEL_HEIGHT = 480;		// Size of height screen that will show the image level, in pixels.
	```  