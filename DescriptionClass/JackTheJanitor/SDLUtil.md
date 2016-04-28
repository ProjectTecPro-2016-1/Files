## CLASS: SDLUtil
Description: Class that draws pictures of elements on a specific position in screen.

### METHODS:
```c++
// -------------------------------------------------------------  
// Function: loadImage()  
// Description: Load image of some element to draw on screen.
// Parameters:
//		string filename;			Name of image file that will be drwan in element.
// Return: SDL_Surface *
// -------------------------------------------------------------
static SDL_Surface * loadImage(std::string filename) {
	...
}
```  

```c++
// -------------------------------------------------------------
// Function: applySurface()
// Description: Applies the surface according to graphic components.
// Parameters:
//		int x;								X axis position where the element will be drawn.
//		int y;								Y axis position where the element will be drawn.
//		SDL_Surface * source;				Pointer to the element that will contain the draw.
//		SDL_Surface * destination;			Pointer to the location where the element is arranged.
//		SDL_Rect * clip;					Null pointer passed as parameter to a graphical function.
// Return: void
// -------------------------------------------------------------
static void applySurface(int x, int y, SDL_Surface * source, SDL_Surface * destination,
						 SDL_Rect * clip = NULL) {
	...
}
```  

### ATTRIBUTES:

### CONST:
