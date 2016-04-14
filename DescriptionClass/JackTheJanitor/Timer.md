## CLASS: Timer
	Description: Class that controls the operation of the time in the game.  

### METHODS:
	```c++
	// -------------------------------------------------------------  
	// Function: Timer()  
	// Description: Builder of the Timer class which hosts the updates of class attributes.  
	// Parameters:  void
	// Attributes: nothing
	// Return: void  
	// -------------------------------------------------------------  
	Timer() {
		...
	}
	```  

	```c++
	// -------------------------------------------------------------  
	// Function: start()  
	// Description: Changes the game status attributes in order to start a new game.  
	// Parameters:  void
	// Attributes: nothing
	// Return: void  
	// -------------------------------------------------------------  
	void start() {
		...
	}
	```  

	```c++
	// -------------------------------------------------------------  
	// Function: stop()  
	// Description: Changes the game status attributes in order to paralyze.  
	// Parameters:  void
	// Attributes: nothing
	// Return: void  
	// -------------------------------------------------------------  
   	void stop() {
		...
	}
	```  

	```c++
	// -------------------------------------------------------------  
	// Function: pause()  
	// Description: Changes the game status attributes in order to pause.  
	// Parameters:  void
	// Attributes: nothing
	// Return: void  
	// -------------------------------------------------------------  
    void pause() {
		...
	}
	```  

	```c++
	// -------------------------------------------------------------  
	// Function: unpause()  
	// Description: Changes the game status attributes in order to take a break.  
	// Parameters:  void
	// Attributes: nothing
	// Return: void  
	// -------------------------------------------------------------  
    void unpause() {
		...
	}
	```  

	```c++
	// -------------------------------------------------------------  
	// Function: waitDiff()  
	// Description: Function that generates a delay in the transition to a frame and another shipment.
	// Parameters:
	//		float ratioFPS;  		Time will the delay.
	// Attributes: nothing
	// Return: void  
	// -------------------------------------------------------------
    void waitDiff(float ratioFPS) {
		...
	}
	```  

	```c++
	// -------------------------------------------------------------  
	// Function: get_ticks()  
	// Description: Returns the time of the current game.
	// Parameters: void
	// Attributes: nothing
	// Return: int  
	// -------------------------------------------------------------
	int get_ticks() {
		...
	}
	```  

	```c++
	// -------------------------------------------------------------  
	// Function: is_started()  
	// Description: Returns information on whether the game is started or not.
	// Parameters: void
	// Attributes: nothing
	// Return: bool  
	// -------------------------------------------------------------
	bool is_started() {
		...
	}
	```  

	```c++
	// -------------------------------------------------------------  
	// Function: is_paused()  
	// Description: Returns information on whether the game is paused or not.
	// Parameters: void
	// Attributes: nothing
	// Return: bool  
	// -------------------------------------------------------------
    bool is_paused() {
		...
	}
	```  

### ATTRIBUTES:
	```c++
	int startTicks;			// Saves the time the game lasted or is lasting.
	int pausedTicks;		// Saves the time the game lasted the rest of the game.
	bool paused;			// It contains information on whether the game is paused or not.
	bool started;			// It contains information on whether the game is started or not.
	```  

### CONST:
