## CLASS: Box
	Description: Class which describes the funcionality of the boxes that the player must escape during the game.  

### METHODS:
	```c++
	// -------------------------------------------------------------  
	// Function: Box()  
	// Description: Box class builder where the inicialization of the class variables happen.  
	// Parameters:  
	//		string fileName;  		Box landscape file name.
	// Return: void  
	// -------------------------------------------------------------  
	Box(std::string filename) {
		...
	}
	```  
	
	```c++
	// -------------------------------------------------------------  
	// Function: ~Box() 
	// Description: Box class destructor where the box image files free themselves.
	// Return: void  
	// -------------------------------------------------------------  
	~Box() {
		...
	}
	```  
	
	```c++
	// -------------------------------------------------------------  
	// Function: drawSelf()  
	// Description: Draws the box in a specific screen position according to the box attributes.
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
	// Function: getPositionX()  
	// Description: Returns a position in the box X axis at the right moment. 
	// Return: int  
	// -------------------------------------------------------------  
	int getPositionX() {
		...
	}
	```  
	
	```c++
	// -------------------------------------------------------------  
	// Function: getPositionY()  
	// Description: Returns a position in the box Y axis at the right moment. 
	// Return: int  
	// -------------------------------------------------------------  
	int getPositionY() {
		...
	}
	```  
	
	```c++
	// -------------------------------------------------------------  
	// Function: getSpeed()  
	// Description: Returns the speed which the box is moving at the right moment. 
	// Return: int  
	// -------------------------------------------------------------  
	int getSpeed() {
		...
	}
	```  
	
	```c++
	// -------------------------------------------------------------  
	// Function: setPosition()  
	// Description: Return the speed which the box is moving at the right moment.
	// Parameters:
	//		int x;			Insert the value of axis X of the box on the attribute that keeps the information
	//		int y;  		Insert the value of axis Y of the box on the attribute that keeps the information	
	// Return: void  
	// -------------------------------------------------------------  
	void setPosition(int x, int y) {
		...
	}
	```  
	
	```c++
	// -------------------------------------------------------------  
	// Function: accelerate()  
	// Description: Increase the speed of the box at the right moment.
	// Return: void
	// Observations:
	// 		- Funtion not implemented
	// -------------------------------------------------------------  
	void accelerate() {
		...
	}
	```  
	
	```c++
	// -------------------------------------------------------------  
	// Function: fall()  
	// Description: Control the box fall during the execution of the level of the game.
	// Parameters:
	//		int vector<Box*> grid[12];			Vector that contain the box positions in the platform.
	// Return: void
	// -------------------------------------------------------------  
	void fall(vector<Box*> grid[12]) {
		...
	}
	```  
	
### ATTRIBUTES:
	```c++
	SDL_Surface * box;		// Pointer for box graphic elements.
    float speed;			// Keep the actual speed of the box.
	bool lyingDown;			// Contain information if the box is falling or not.
	int xPosition;			// Keep the actual position of the box on axis X.
	int yPosition;			// Keep the actual position of the box on axis Y.
	bool used;				// Contain information if the box is already in the game or not.
	```  

### CONST:
	```c++
	static const int BOX_WIDTH = 38;		// All boxes pixel width.
	static const int BOX_HEIGHT = 38;		// All boxes pixel height.
	static const int ACCELERATION = 1;		// Used for increments the box speed after the creation of each box.
    static const int MAX_SPEED = 3;			// Keep the information about the maximum speed that the box can achieve.
	```  