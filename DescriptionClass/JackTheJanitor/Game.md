## CLASS: Game
	Description: It's the most important class of the project. It's does all operation need to game 
				start and run, and has control of the operations in the game.
	Observation: Main.cpp call this class.

### METHODS:
	```c++
	// -------------------------------------------------------------
	// Function: init()
	// Description: Function that initialize atributtes on game and calls other function to initalize 	
	//				graphic properties.
	// Return: void
	// -------------------------------------------------------------
	void init() {
		...
	}
	```  

	```c++
	// -------------------------------------------------------------
	// Function: loop()
	// Description: On game operation generate a cycle. To keeps control of execution inside a function 	//				on game.
	// Return: void
	// -------------------------------------------------------------
	void loop() {
		...
	}
	```  

	```c++
	// -------------------------------------------------------------
	// Function: shutdown()
	// Description:	Clean graphic and audio components, ending the 
	//				execution of the game.
	// Return: void
	// -------------------------------------------------------------
	void shutdown() {
		...
	}
	```  

	```c++
	// -------------------------------------------------------------
	// Function: initGUI()
	// Description: Needed to center the startup oh the graphical interface
	//				of policy controlled by SDL.
	// Return: void
	// -------------------------------------------------------------
	void initGUI() {
		...
	}
	```  

	```c++
	// -------------------------------------------------------------
	// Function: closeGUI()
	// Description: Needed to center the completion of audio and image
	//				plugins from SDL libraries. 
	// Return: void
	// -------------------------------------------------------------
	void closeGUI() {
		...
	}
	```  

	```c++
	// -------------------------------------------------------------
	// Function: wonGameScreen()
	// Description: Load and show on screen a image of won game.
	//				Only runs when the game ends with victory.
	// Attributes:
	// 		bool playButton;		Contains the information if the button to start a new
	//								game was clicked or not.
	//		bool quitButton;		Contains the information if the button to exit was 
	//								clicked or not.
	// Return: void
	// -------------------------------------------------------------
	void wonGameScreen() {
		...
	}
	```  

	```c++
	// -------------------------------------------------------------
	// Function: showOptionsScreen()
	// Description:	Load and show a image and Screen Options of game along
	//				with the buttons that are part of the same.
	// Attributes:
	// 		bool muteButton;		Information about button of audio enable or
	//								disable it was clicked or not.
	//		bool loadButton;		Information about button to load a game it was clicked or not.
	//		bool backButton;		Information about button that returns to previous screen it was
	//								clicked or not.
	// Return: void
	// -------------------------------------------------------------
	void showOptionsScreen() {
		...
	}
	```  

	```c++
	// -------------------------------------------------------------
	// Function: gameOvering()
	// Description: When Jack dies or game is finished this function is called.
	// Return: void
	// -------------------------------------------------------------
	void gameOvering() {
		...
	}
	```  

	```c++
	// -------------------------------------------------------------
	// Function: gameOverScreenDraw()
	// Description: From gameOvering function it is intended to present
	//				the GameOver screen to the user.
	// Return: void
	// -------------------------------------------------------------
	void gameOverScreenDraw() {
		...
	}
	```  

	```c++
	// -------------------------------------------------------------
	// Function: gameOverScreenLoop()
	// Description: On GameOver screen generates a loop to wait an action of the player. 
	// Attributes:
	// 		bool playButton;		Contains information about Start Game Button it was clicked or 
	//								not.
    //		bool quitButton;		Contains information about Exit Game Button it was clicked or 
    //								not.
    //		bool optionsButton;		Contains information about Options Game Button it was clicked or
    //								not.
	// Return: void
	// -------------------------------------------------------------
	void gameOverScreenLoop() {
		...
	}
	```  

	```c++
	// -------------------------------------------------------------
	// Function: pausingLevel()
	// Description: This function is called when Pause Game Button is clicked on game execution.
	// Return: void
	// -------------------------------------------------------------
	void pausingLevel() {
		...
	}
	```  

	```c++
	// -------------------------------------------------------------
	// Function: pauseScreenDraw()
	// Description: From pausingLevel function and it is intended to shows Pause Screen to the user.
	// Return: void
	// -------------------------------------------------------------
	void pauseScreenDraw() {
		...
	}
	```  

	```c++
	// -------------------------------------------------------------
	// Function: pauseScreenLoop()
	// Description: Genarates on Pause Screen a loop while waiting an action of the player. 
	// Attributes: 
	// 		bool playButton;		Contains information about Return Game Button it was clicked or 
	//								not.
    //		bool quitButton;		Contains information about Exit Game Button it was clicked or 
    //								not.
    //		bool optionsButton;		Contains information about Options Game Button
    //								it was clicked or not.
	// Return: void
	// -------------------------------------------------------------
	void pauseScreenLoop() {
		...
	}
	```  

	```c++
	// -------------------------------------------------------------
	// Function: initializingScreen()
	// Description: Initialize the process of show on Initial Screen, alomg with startup of audios.
	// Return: void
	// -------------------------------------------------------------
	void initializingScreen() {
		...
	}
	```  

	```c++
	// -------------------------------------------------------------
	// Function: initScreenDraw()
	// Description: From initializingScreen function and it is intended to shows
	//				Init Screen to user.
	// Return: void
	// -------------------------------------------------------------
	void initScreenDraw() {
		...
	}
	```  

	```c++
	// -------------------------------------------------------------
	// Function: initScreenLoop()
	// Description: Generates on Init Screen a loop while waiting an action from user.
	// Attributes:
	// 		bool playButton;		Contains information about Start New Game Button it was cliked 
	//								or not.
    //		bool quitButton;		Contains information about End Game Button it was clicked or 
    //								not.
    //		bool optionsButton;		Contains information about Options Menu Button it was clicked or
    //								not.
	// Return: void
	// -------------------------------------------------------------
	void initScreenLoop() {
		...
	}
	```   

	```c++
	// -------------------------------------------------------------
	// Function: loadCommonResources()
	// Description: Initialize common resources for game, like audio and sound.
	// Return: void
	// -------------------------------------------------------------
	void loadCommonResources() {
		...
	}
	```  

	```c++
	// -------------------------------------------------------------
	// Function: releaseCommonResources()
	// Description: Common resoucers are cleaned and released by this function.
	// Return: void
	// Observations:
	// 		Funtion not implemented
	// -------------------------------------------------------------
	void releaseCommonResources() {
		...
	}
	```  

	```c++
	// -------------------------------------------------------------
	// Function: loadProfile()
	// Description: Load a profile that stores data for a specific user.
	// Return: void
	// Observations:
	// 		Funtion not implemented
	// -------------------------------------------------------------
	void loadProfile() {
		...
	}
	```  

	```c++
	// -------------------------------------------------------------
	// Function: saveProfile()
	// Description: A user profile is saved to be used in another time.
	// Return: void
	// Observations:
	// 		Funtion not implemented
	// -------------------------------------------------------------
	void saveProfile() {
		...
	}
	```  

	```c++
	// -------------------------------------------------------------
	// Function: loadLevel()
	// Description: All informations about user level is loaded, like each enemy image, Jack image, 						during execution quantity of boxes that will fall, audios and score. 
	// Attributes:
	//		string level_1_file;		Background filename from level 1.
	//	    string level_2_file;		Background filename from level 2.
	//	    string level_3_file;		Background filename from level 3.
	//	    string level_1_spec;		Filename that contains specifications about level 1.
	//	    string level_2_spec;		Filename that contains specifications about level 2.
	//	    string level_3_spec;		Filename that contains specifications about level 3.
	//	    string currentLevelFile;	Image filename about actual level.
	//	    string currentLevelSpec;	Filename that contains specifications about acutal level.
	//		ifstream levelFile;			Controls file of level specifications.
    //		string numberOfLevel;		It contains the number of level read in levelFile .
    //		string numberOfBoxes;		Read on levelFile, contains the number of boxes that 
    //									level will 	have.
    //		string numberOfEnemies;		Read on levelFile, contains the number of enemies that
    //									level will have.
    //		string maxLines;			Read on levelFile, contains the necessary number of lines 
    //									filled with boxes pass the level.
    //		int nrBoxes;				Contais a integer number stemmed from numberOfBoxes 
    //									variable.
    //		int nrEnemies;				Contais a integer value stemmed from numberOfEnemies 
    //									varible.
	// Return: void
	// -------------------------------------------------------------
	void loadLevel() {
		...
	}
	```  

	```c++
	// -------------------------------------------------------------
	// Function: releaseLevel()
	// Description: Actual level is deleted freeing up memory to the next level to load.
					Deleta o nível atual liberando memória para o próximo nível ser carregado.
	// Return: void
	// -------------------------------------------------------------
	void releaseLevel() {
		...
	}
	```  

	```c++
	// -------------------------------------------------------------
	// Function: updateTimeStep()
	// Description: Run so a level ends, initializing a new time of game.
	// Return: void
	// -------------------------------------------------------------
	void updateTimeStep() {
		...
	}
	```  

	```c++
	// -------------------------------------------------------------
	// Function: update()
	// Description: Updates atributtes of control on game during the game loop.
	// Return: void
	// -------------------------------------------------------------
	void update() {
		...
	}
	```  

	```c++
	// -------------------------------------------------------------
	// Function: draw()
	// Description: Focuses the creation and printing of background images from ScoreScreen
	//				and LevelScreen.
	// Return: void
	// -------------------------------------------------------------
	void draw() {
		...
	}
	```  

	```c++
	// -------------------------------------------------------------
	// Function: runAI()
	// Description: Generates the movement of enemies and locations where they will drop boxes.
	// Return: void
	// -------------------------------------------------------------
	void runAI() {
		...
	}
	```  

	```c++
	// -------------------------------------------------------------
	// Function: runPhysics()
	// Description: Collisions, falls, movements from boxes and players, the physics from actions
	//				are executed on here.
	// Attributes:
	//		int xinit;		Saves the X position where you begin drawing level.(minimum left)
	//	    int xrange;		Saves the X position where you end drawing level.(maximum right)
	//	    int jackposx;					Keeps Jacks postition on X.
	//	    int jackposy;					Keeps Jacks position on Y.
	//	    int boxMobileBeforeJack;		Saves the first box position before Jack.
	//	    int boxMobileAfterJack;			Saves the first box position after Jack.
	//		int quantidadeDeCaixas;			Contains information about quantity of boxes on base 
	//										line.
	//		Box * boxToDelete;				Controls which boxes will be deleted when tha base line 
	//										was complete with 12 boxes.	
	//		Box * boxTransition;			Controls the box will be moved to the left.
	//		Box * boxTransitionRight;		Controls the box will be moved to the right.
	// Return: void
	// -------------------------------------------------------------
	void runPhysics() {
		...
	}
	```  

	```c++
	// -------------------------------------------------------------
	// Function: recieveNetworkData()
	// Description:
	// Return: void
	// Observations:
	// 		Funtion not implemented
	// -------------------------------------------------------------
	void recieveNetworkData() {
		...
	}
	```  

	```c++
	// -------------------------------------------------------------
	// Function: sendNetworkData()
	// Description:
	// Return: void
	// Observations:
	// 		Funtion not implemented
	// -------------------------------------------------------------
	void sendNetworkData() {
		...
	}
	```  

	```c++
	// -------------------------------------------------------------
	// Function: handleEventMouseButtonUp()
	// Description: Performs the action of the click of a mouse button.
	//				After pressing the button, release the button.	
	// Parameters:
	//		SDL_Event & event;		Contains information about some action on mouse made by user.
	// Return: void
	// -------------------------------------------------------------
	void handleEventMouseButtonUp(SDL_Event & event) {
		...
	}
	```  

	```c++
	// -------------------------------------------------------------
	// Function: handleEventMouseButtonDown()
	// Description:	Performs the click action of some button on mouse.
	//				Button pressed.
	// Parameters:
	//		SDL_Event & event;		Contains information about some action on mouse made by user.
	// Return: void
	// -------------------------------------------------------------
	void handleEventMouseButtonDown(SDL_Event & event) {
		...
	}
	```  

	```c++
	// -------------------------------------------------------------
	// Function: handleEventKeyDown()
	// Description: Performs the action of click in any key on the keyboard.
	//				Button pressed.
	// Parameters:
	//		SDL_Event & event;		Contains information about some action made by user.
	// Return: void
	// -------------------------------------------------------------
	void handleEventKeyDown(SDL_Event & event) {
		...
	}
	```

	```c++
	// -------------------------------------------------------------
	// Function: handleEventKeyUp()
	// Description:	Performs the action of click in any key on the keyboard. 
	//				After pressing the button, release the button.	
	// Parameters:
	//		SDL_Event & event;		Contains information about some action made by user.
	// Return: void
	// -------------------------------------------------------------
	void handleEventKeyUp(SDL_Event & event) {
		...
	}
	```

	```c++
	// -------------------------------------------------------------
	// Function: handleEventType()
	// Description:	Identifies which type of action is made by user and sends to the specific
	//				function that will treat.
	// Parameters:
	//		SDL_Event & event;		Contains information about some action made by user.
	// Return: void
	// -------------------------------------------------------------
	void handleEventType(SDL_Event & event) {
		...
	}
	```

	```c++
	// -------------------------------------------------------------
	// Function: handleEvents()
	// Description: Identifies and call handleEventType function to treat an action made by user
	//				on mouse or keyboard.
	// Return: void
	// -------------------------------------------------------------
	void handleEvents() {
		...
	}
	```  
	
	```c++
	// -------------------------------------------------------------
	// Function: checkIfSkip()
	// Description: Checks if frame was loaded, if not wait the frame load.
	// Return: int
	// -------------------------------------------------------------
	int checkIfSkip() {
		...
	}
	```  

	```c++
	// -------------------------------------------------------------
	// Function: checkColision()
	// Description: It performs checks whether or not collision between Jack and the boxes.
	// Parameters:
	//		Jack * jack;				Used to acess informations, it is a pointer to Jack.
	//		std::vector<Box*> boxes;	Pointer to existing boxes during the game.
	// Attributes:
	//		int jackRight;				Position and limit x from right side of Jack.
	//		int jackLeft;				Position and limit x from left side of Jack .
	//		int jackTop;				Position and limit y from upper side of Jack.
	//		int jackBottom;				Position and limit y from lower side of Jack.
	//		int boxRight;				Position and limit x from right side of box to be 
	//									checked.
	//		int boxLeft;				Position and limit x from left side of box to be 
	//									checked.
	//		int boxTop;					Position and limit y from upper side of box to be 
	//									checked.
	//		int boxBottom;				Position and limit y from lower side of box to be 
	//									checked.
	// Return: bool
	// -------------------------------------------------------------
	bool checkColision(Jack * jack, std::vector<Box*> boxes) {
		...
	}
	```  

	```c++
	// -------------------------------------------------------------
	// Function: isGameFinished()
	// Description: Check if player ordered the game closing.
	// Return: bool
	// -------------------------------------------------------------
	bool isGameFinished() {
		...
	}
	```  

	```c++
	// -------------------------------------------------------------
	// Function: isLevelFinished()
	// Description:	Check if player end the actual level.
	// Return: bool
	// -------------------------------------------------------------
	bool isLevelFinished() {
		...
	}
	```  

### ATRIBUTTES:
	```c++
	SDL_Surface * screen;					// Main Screen that will show graphic elements.
	SDL_Event event;						// Keeps user action if exists.
	Jack * jack;							// Pointer that keeps informationa bout Jack.
	Level * level;							// Keep informations about actual level.
	Timer frameTime;						// Controls loading and time of frames.
	ScoreScreen * score;					// Centralizes informations about score on game.
	InitScreen * initScreen;				// Keep informations about Initial Screen.
	InitScreen * wonScreen;					// Controls the Won Game Screen which is executed at the
	 										// end of each level.
	PauseScreen * pauseScreen;				// Controls the Pause Screen when user execute.
	GameOverScreen * gameOverScreen;		// Controls the Game Over Screen which is executed at 
											// the end of each level.
	OptionsScreen * optionsScreen;			// Controls Options Screen.
	Label * labelPlay;						// Play Button on game.
	Label * labelOptions;					// Options Button on game.
	Label * labelQuit;						// Button that end game or cancels execution of some 
											// level.
	Label * labelMute;						// Button from Options Screen that allows audio  
											// execution or not.
	Label * labelLoad;						// Button from Options Screen that load a new game.
	Label * labelBack;						// Button from Options Screen that returns to Initial
											// Screen.
	float FRAME_MILISECOND;					// It contains the millisecond transition from one frame
											// to another
	bool quitGame;							// Information if the user wants to leave or not the 
											// game.
	bool quitLevel;							// Information if necessary leave or not the level.
	bool pauseLevel;						// Inforamtion if the game is paused or not.
	bool gameOver;							// Information if the player lost or not the game.
	bool gameWon;							// Information if the player won or not the game. 
	int linesDeleted;						// Number of lines that have been completed by the 
											// player.
	int maxLevelLines;						// Number of lines that is necessary to won the game.
	int actualLevel;						// Contains the actual level number of player o game.
	```  

### CONST:
	```c++
	static const int SCREEN_WIDTH = 854;		// Size width of the game screen.
	static const int SCREEN_HEIGHT = 480;		// Size game screen height.
	static const int SCREEN_BPP = 32;			// Number of bits per pixel permitted in the screen.
	static const int SCREEN_FPS = 60;			// Number of frames per second allowed.
	```  
