## CLASS: Timer
	Description: Class that controls the action of the time on game.

### METHODS:
	```c++
	// -------------------------------------------------------------  
	// Function: Timer()  
	// Description: Class Time constructor where that happens attributes  inicialization.
	// Parameters:  void
	// Atributes: nothing
	// Return: void  
	// -------------------------------------------------------------  
	Timer() {
		...
	}
	```  
	
	```c++
	// -------------------------------------------------------------  
	// Function: start()  
	// Description: Change the status of attributes on game  in order to start a new game.  
	// Parameters:  void
	// Atributes: nothing
	// Return: void  
	// -------------------------------------------------------------  
	void start() {
		...
	}
	```  
	
	```c++
	// -------------------------------------------------------------  
	// Function: stop()  
	// Description: Change the status of attributes on game in order to paralyze.
	// Parameters:  void
	// Atributes: nothing
	// Return: void  
	// -------------------------------------------------------------  
   	void stop() {
		...
	}
	```  
	
	```c++
	// -------------------------------------------------------------  
	// Function: pause()  
	// Description: Change the status of attributes on game in order to stop.
	// Parameters:  void
	// Atributes: nothing
	// Return: void  
	// -------------------------------------------------------------  
    void pause() {
		...
	}
	```  
	
	```c++
	// -------------------------------------------------------------  
	// Function: unpause()  
	// Description: Change the status of attributes on game in order to take the "pause".
	// Parameters:  void
	// Atributes: nothing
	// Return: void  
	// -------------------------------------------------------------  
    void unpause() {
		...
	}
	```  
	
	```c++
	// -------------------------------------------------------------  
	// Function: waitDiff()  
	// Description: Function that generates a delay between frames.
	// Parameters:
	//		float ratioFPS;  		Time of delay.
	// Atributes: nothing
	// Return: void  
	// ------------------------------------------------------------- 
    void waitDiff(float ratioFPS) {
		...
	}
	```  
	
	```c++
	// -------------------------------------------------------------  
	// Function: get_ticks()  
	// Description: Returns the instant of actual game.
	// Parameters: void
	// Atributes: nothing
	// Return: int  
	// ------------------------------------------------------------- 
	int get_ticks() {
		...
	}
	```  
	
	```c++
	// -------------------------------------------------------------  
	// Function: is_started()  
	// Description: Returns the information if the game has been initialized or not.
	// Parameters: void
	// Atributes: nothing
	// Return: bool  
	// ------------------------------------------------------------- 
	bool is_started() {
		...
	}
	```  
	
	```c++
	// -------------------------------------------------------------  
	// Function: is_paused()  
	// Description: Returns the information is the game is paused or not.
	// Parameters: void
	// Atributes: nothing
	// Return: bool  
	// ------------------------------------------------------------- 
    bool is_paused() {
		...
	}
	```  
	
### ATTRIBUTES:
	```c++
	int startTicks;			// Keeps the time of the game or the time it is lasting.
	int pausedTicks;		// Keep the time of long last pause.
	bool paused;			// Contains a information if the game is paused or not.
	bool started;			// Contains a information if the game has been initialized or not.
	```  

### CONST: