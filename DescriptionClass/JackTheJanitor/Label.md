## CLASS: Label
	Description: Class which describes the funcionality of the labels during the game.  

### METHODS:
	```c++
	// -------------------------------------------------------------  
	// Function: Label()  
	// Description: Label class builder where the inicialization of the class variables happen.
	// Parameters:
	//		string filename;		Label landscape file name.
	//		int xPosition;			Where the label is localizated in axis X.
	//		int yPosition;			Where the label is localizated in axis Y
	// Return: void  
	// -------------------------------------------------------------  
	Label(std::string filename, int xPosition, int yPosition) {
		...
	}
	```  
	
	```c++
	// -------------------------------------------------------------  
	// Function: ~Label()  
	// Description: Label class destructor where the level image files free themselves.
	// Return: void  
	// -------------------------------------------------------------  
	~Label() {
		...
	}
	```  
	
	```c++
	// -------------------------------------------------------------  
	// Function: drawSelf()  
	// Description: Draws the label on the specified surface.
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
	// Function: wasClicked()  
	// Description: Where was clicked by the user
	// Parameters:
	//		int xMouse;		Where the mouse is localizated in axis X.
	//		int yMouse;		Where the mouse is localizated in axis Y.
	// Return: bool
	// -------------------------------------------------------------  
	bool wasClicked(int xMouse, int yMouse) {
		...
	}
	```  
	
### ATRIBUTTES:
	```c++
	SDL_Surface *label;			// Pointer for label graphic elements.
	int xPosition;				// Where the label is localizated in axis X.
	int yPosition;				// Where the label is localizated in axis Y.
	```  
	
### CONST:
	```c++
	static const int LABEL_WIDTH = 178;		// All label pixel width.
	static const int LABEL_HEIGHT = 100;		// All label pixel heigth.
	```  
