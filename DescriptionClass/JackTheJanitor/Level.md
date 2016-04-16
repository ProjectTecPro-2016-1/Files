## CLASS: Level
	Description: Class which describes the funcionality of the levels during the game.  
	
### METHODS:
	```c++
	// -------------------------------------------------------------  
	// Function: Level()  
	// Description: Level class builder where the inicialization of the class variables happen.
	// Parameters:
	//		string filename;		Level landscape file name.
	// Return: void  
	// -------------------------------------------------------------  
	Level(std::string filename) {
		...
	}
	```  
	
	```c++
	// -------------------------------------------------------------  
	// Function: ~Level()  
	// Description: Level class destructor where the level image files free themselves.
	// Return: void  
	// -------------------------------------------------------------  
   	~Level() {
		...
	}
	```  
	
	```c++
	// -------------------------------------------------------------  
	// Function: drawSelf()  
	// Description: Draws the level in a specific screen position according to the box attributes.
	// Parameters:
	//		SDL_Surface * surface;		Pointer for the surface where the graphic component will be drawn.
	// Return: void  
	// -------------------------------------------------------------  
	void drawSelf(SDL_Surface * surface) {
		...
	}
	```  
	
	```c++
	// -------------------------------------------------------------  
	// Function: getBoxes()  
	// Description: Returns a vector whith all box positions.
	// Return: vector<Box*>  
	// -------------------------------------------------------------  
	vector<Box*> getBoxes() {
		...
	}
	```  
	
### ATTRIBUTES:
	```c++
	SDL_Surface * level;			// Pointer for level graphic elements.
	vector<Enemy*> enemies;			// Vector that contains info about enemies.
	vector<Box*> boxes;				// Vector that contains info about boxes.
	vector<Box*> grid[12];			// Vector that contains the platform where the box falls.
	```  
	
### CONST:
	```c++
	static const int LEVEL_WIDTH = 456;			// All level pixel width.
	static const int LEVEL_HEIGHT = 456;		// All level pixel height.
	static const int LEVEL_X_OFFSET = 50;		// Where the level is drawn on the specified surface in axis X.
	static const int LEVEL_Y_OFFSET = 10;		// Where the level is drawn on the specified surface in axis Y.
	```  