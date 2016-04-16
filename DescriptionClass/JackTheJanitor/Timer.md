## CLASS: Timer
	Description: Class that controls the operation of the time in the game.  

### METHODS:
	```c++
	// -------------------------------------------------------------  
	// Function: Timer()  
	// Description: Builder of the Timer class which hosts the updates of class attributes.  
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
