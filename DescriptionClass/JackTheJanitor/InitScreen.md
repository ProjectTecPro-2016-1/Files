## CLASS: InitScreen
	Description: Controls all actions that the screen runs at the beginning of the game.

### METHODS:
	```c++
	// -------------------------------------------------------------  
	// Function: InitScreen()  
	// Description: Load the image of Start Game, the initial screen.
	// Parameters:
	//		string filename;		Name of "initial" image file that will be showed on screen.
	// Return: void  
	// -------------------------------------------------------------  
	InitScreen(std::string filename) {
		...
	}
	```  
	
	```c++
	// -------------------------------------------------------------  
	// Function: ~InitScreen()  
	// Description: Destructor of class that clean the initial screen.
	// Return: void  
	// -------------------------------------------------------------  
	~InitScreen() {
		...
	}
	```  
	
	```c++
	// -------------------------------------------------------------  
	// Function: drawSelf()  
	// Description: Applies the image of Start Game on screen.
	// Parameters:
	//		SDL_Surface *surface;		Is the surface that the image will load.
	// Return: void  
	// -------------------------------------------------------------  
	void drawSelf(SDL_Surface *surface) {
		...
	}
	```  

### ATRIBUTTES:
	```c++
	SDL_Surface *initScreen;		// Keeps the image that loaded.
	```  
	
### CONST:
	```c++
	static const int LEVEL_WIDTH = 854;			// Size of width screen that will show the image level, in pixels.
    static const int LEVEL_HEIGHT = 480;		// Size of height screen that will show the image level, in pixels.
	```  