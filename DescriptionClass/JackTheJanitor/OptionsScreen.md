## CLASS: OptionsScreen
	Description: Controls all actions that be displayed for the player about "Help" an "Options" of the game.
	
### METHODS:
	```c++
	// -------------------------------------------------------------  
	// Function: OptionsScreen()  
	// Description: Load the image of "Help" and "Options".
	// Parameters:
	//		string filename;		Name of image file that will be showed on screen.
	// Return: void  
	// -------------------------------------------------------------  
	OptionsScreen(std::string filename) {
		...
	}
	```  
	
	```c++
	// -------------------------------------------------------------  
	// Function: ~OptionsScreen()  
	// Description: Destructor of class that clean the screen of options and screen of help.
	// Return: void  
	// -------------------------------------------------------------  
	~OptionsScreen() {
		...
	}
	```  
	
	```c++
	// -------------------------------------------------------------  
	// Function: drawSelf()  
	// Description: Applies the image of "Help" and "Options" on screen.
	// Parameters:
	//		SDL_Surface *surface;		Is the surface that the image will load.
	// Attributes: nothing
	// Return: void  
	// -------------------------------------------------------------  
	void drawSelf(SDL_Surface *surface) {
		...
	}
	```  

### ATTRIBUTES:
	```c++
	SDL_Surface *helpMessage;
	SDL_Surface *optionsScreen;
	static const int SCREEN_WIDTH = 854;
	static const int SCREEN_HEIGHT = 480;
	```  

### CONST: