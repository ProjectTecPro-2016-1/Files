## CLASS: GameObject
	Description: Abstract class in which are declared the methods responsible to put objects on the screen

### METHODS:
	```c++
	// -------------------------------------------------------------
	// Function: ~GameObject()
	// Description: Virtual class destructor method
	// Parameters: void
	// Attributes: nothing
	// Return: void
	// -------------------------------------------------------------
	virtual ~GameObject() {
		...
	}
	```

	```c++
	// -------------------------------------------------------------
	// Function: draw()
	// Description: Method that draws a object on the screen
	// Parameters:
	//		SDL_Surface *surface;		Pointer for the surface where the graphic component will be drawn.
	// Attributes: nothing
	// Return: void
	// -------------------------------------------------------------
	void draw(SDL_Surface *surface) {
		...
	}
	```

	```c++
	// -------------------------------------------------------------
	// Function: addChild()
	// Description: Adds a element to the vector GamesObject*
	// Parameters:
	//		GameObject* child;		Pointer to the game object in question
	// Attributes: nothing
	// Return: void
	// -------------------------------------------------------------
	void addChild(GameObject* child) {
		...
	}
	```

	```c++
	// -------------------------------------------------------------
	// Function: drawSelf()
	// Description: Draws the game object in a specific screen position according to the box attributes.
	// Parameters:
	//		SDL_Surface *surface;		Pointer for the surface where the graphic component will be drawn.
	// Attributes: nothing
	// Return: void
	// -------------------------------------------------------------
	virtual void drawSelf(SDL_Surface *surface) == 0;
	```

### ATRIBUTTES:
	```c++
	vector<GameObject*> children; // Vector that stocks the objects of the game
	```

### CONST:
