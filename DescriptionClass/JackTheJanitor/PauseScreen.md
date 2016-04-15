## CLASS: PauseScreen
	Description: Controls whats is displayed on the screen for the player when the game is paused.
	
### METHODS:
	```c++
	// -------------------------------------------------------------  
	// Function: PauseScreen()  
	// Description: Load the image of Pause on game.
	// Parameters:
	//		string filename;		Name of "pause" image file that will be showed on screen.
	// Return: void  
	// -------------------------------------------------------------  
	PauseScreen(std::string filename) {
		...
	}
	```  
	
	```c++
	// -------------------------------------------------------------  
	// Function: ~PauseScreen()  
	// Description: Destructor of class that clean the pause screen.
	// Return: void  
	// -------------------------------------------------------------  
    ~PauseScreen() {
		...
	}
	```  
	
	```c++
	// -------------------------------------------------------------  
	// Function: drawSelf()  
	// Description: Applies the image of Pause Game on screen.
	// Parameters:
	//		SDL_Surface *surface;		Is the surface that the image will load.
	// Return: void  
	// -------------------------------------------------------------  
	void drawSelf(SDL_Surface *surface) {
		...
	}
	```  

### ATTRIBUTES:
	```c++
	SDL_Surface * pauseScreen;					// Surface for "Pause" that will be applie on screen.
	```  
	
### CONST:
	```c++
	static const int LEVEL_WIDTH = 854;			// Size of width screen that will show the image level, in pixels.
    static const int LEVEL_HEIGHT = 480;		// Size of height screen that will show the image level, in pixels.
	```