## CLASS: RawImage
	Description: Class that controls images.
	
### METHODS:
	```c++
	// -------------------------------------------------------------  
	// Function: RawImage()  
	// Description: Image class builder where the initialization of the class variable happen.
	// Return: void  
	// -------------------------------------------------------------  
	RawImage() {
		...
	}
	```  
	
	```c++
	// -------------------------------------------------------------  
	// Function: ~RawImage()  
	// Description: Image class destructor where the image files free themselves.
	// Return: void  
	// -------------------------------------------------------------  
	~RawImage() {
		...
	}
	```  
	
	```c++
	// -------------------------------------------------------------  
	// Function: load()  
	// Description: Load the images on surface if its not empty.
	// Parameters:
	// 		const string & name;			File name.
	// Return: void  
	// -------------------------------------------------------------  
	void load(const string & name) {
		...
	}
	```  
	
	```c++
	// -------------------------------------------------------------  
	// Function: width()  
	// Description: Keep image width.
	// Return: int
	// -------------------------------------------------------------  
	int width() const {
		...
	}
	```  
	
	```c++
	// -------------------------------------------------------------  
	// Function: height()  
	// Description: Keep image height.
	// Return: int
	// -------------------------------------------------------------  
	int height() const {
		...
	}
	```  
	
	```c++
	// -------------------------------------------------------------  
	// Function: pixels()  
	// Description: Return surface.
	// Return: SDL_Surface *	
	// -------------------------------------------------------------  
	SDL_Surface * pixels() const {
		...
	}
	```	 

### ATTRIBUTES:
	```c++
	SDL_Surface * _pixels;		// Pointer for pixels graphic elements.
	```  

### CONST: