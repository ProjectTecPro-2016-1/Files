## CLASS: SDLUtil
	Description: Class that draws pictures of elements on a specific position in screen.
	
### METHODS:
    ```c++
	// -------------------------------------------------------------  
	// Function: loadImage()  
	// Description: Load image of some element to draw on screen.
	// Parameters:
	//		string filename;			Name of image file that will be drwan in element.
	// Atributes: nothing
	// Return: void
	// ------------------------------------------------------------- 
	static SDL_Surface *loadImage(std::string filename) {
		...
	}
	```  
	
	```c++
	// -------------------------------------------------------------  
	// Function: applySurface()  
	// Description: Apply the interface according to grafic components. 
	// Parameters:
	//		int x;								Position on the X axis where the element will be draw.
	//		int y;								Position on the Y axis where where the element will be draw.
	//		SDL_Surface *source;				Pointer to the element that will contain the drawning.
	//		SDL_Surface *destination;			Pointer to the location where the element will be disposed.
	//		SDL_Rect* clip;						Not know. 
	// Atributes: nothing
	// Return: void
	// ------------------------------------------------------------- 
	static void applySurface(int x, int y, SDL_Surface *source, SDL_Surface *destination, SDL_Rect* clip = NULL) {
		...
	}
	```  
	
### ATTRIBUTES:

### CONST: