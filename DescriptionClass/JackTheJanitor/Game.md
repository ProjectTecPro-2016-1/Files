## CLASS: Game
	Description: It's the most important class of the project. It's does all operation need to game start and run, and has control of the operations in the game.
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
	// 		bool playButton;		Contains information about Start Game Button it was clicked or not.
    //		bool quitButton;		Contains information about Exit Game Button it was clicked or not.
    //		bool optionsButton;		Contains information about Options Game Button it was clicked or not.
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
	// 		bool playButton;		Contains information about Return Game Button it was clicked or not.
    //		bool quitButton;		Contains information about Exit Game Button it was clicked or not.
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
->	// Description: 
					Inicia o processo de mostrar a tela de início do jogo 
	//				juntamente com a inicialização dos áudios.
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
	// 		bool playButton;		Contains information about Start New Game Button it was cliked or not.
    //		bool quitButton;		Contains information about End Game Button it was clicked or not.
    //		bool optionsButton;		Contains information about Options Menu Button it was clicked or not.
	// Return: void
	// -------------------------------------------------------------
	void initScreenLoop() {
		...
	}
	```   

	```c++
	// -------------------------------------------------------------
	// Function: loadCommonResources()
	// Description: 
->					Faz a inicialização dos recursos comuns de funcionamento do jogo, como som e áudio.
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
	// Description: All informations about user level is loaded, like each enemy image, Jack image, during 					execution quantity of boxes that will fall, audios and score. 
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
    //		string maxLines;			Read on levelFile, contains the necessary number of lines filled
    //									with boxes pass the level.
    //		int nrBoxes;				Contais a integer number stemmed from numberOfBoxes variable.
    //		int nrEnemies;				Contais a integer value stemmed from numberOfEnemies varible.
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
	// Description: Collisions, falls, movements from boxes and players, the physics from actions are 		//				executed on here.
	// Attributes:
	//		int xinit;		Guarda a posição X de onde inicia o desenho do nível. (Limite mínimo a esquerda)
	//	    int xrange;		Guarda a posição X de onde termina o desenho do nível. (Limite máximo a direita)
	//	    int jackposx;					Guarda a posição em X do boneco Jack.
	//	    int jackposy;					Guarda a posição em Y do boneco Jack.
	//	    int boxMobileBeforeJack;		Guarda a posição onde tem a primeira caixa antes do boneco Jack.
	//	    int boxMobileAfterJack;			Guarda a posição onde tem a primeira caixa após o boneco Jack.
	//		int quantidadeDeCaixas;			Contém informação de quantas caixas existem na linha base.
	//		Box * boxToDelete;				Controla as caixa que serão deletadas quando a linha base 
	//										está completa com 12 caixas.
	//		Box * boxTransition;			Controla a caixa que será movida para a esquerda.
	//		Box * boxTransitionRight;		Controla a caixa que será movida para a direita.
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
	// Description: Executa a ação do clique de algum botão do mouse.
	//				Após pressionar o botão, soltar o botão.
	// Parameters:
	//		SDL_Event & event;		Contém a informação de algum ação que aconteceu efetuado pelo usuário.
	// Return: void
	// -------------------------------------------------------------
	void handleEventMouseButtonUp(SDL_Event & event) {
		...
	}
	```  

	```c++
	// -------------------------------------------------------------
	// Function: handleEventMouseButtonDown()
	// Description:	Executa a ação do clique de algum botão do mouse.
	//				Botão pressionado.
	// Parameters:
	//		SDL_Event & event;		Contém a informação de algum ação que aconteceu efetuado pelo usuário.
	// Return: void
	// -------------------------------------------------------------
	void handleEventMouseButtonDown(SDL_Event & event) {
		...
	}
	```  

	```c++
	// -------------------------------------------------------------
	// Function: handleEventKeyDown()
	// Description: Executa a ação do clique de alguma tecla do teclado.
	//				Botão pressionado.
	// Parameters:
	//		SDL_Event & event;		Contém a informação de algum ação que aconteceu efetuado pelo usuário.
	// Return: void
	// -------------------------------------------------------------
	void handleEventKeyDown(SDL_Event & event) {
		...
	}
	```

	```c++
	// -------------------------------------------------------------
	// Function: handleEventKeyUp()
	// Description:	Executa a ação do clique de alguma tecla do teclado.
	//				Após pressionar o botão, soltar o botão.
	// Parameters:
	//		SDL_Event & event;		Contém a informação de algum ação que aconteceu efetuado pelo usuário.
	// Return: void
	// -------------------------------------------------------------
	void handleEventKeyUp(SDL_Event & event) {
		...
	}
	```

	```c++
	// -------------------------------------------------------------
	// Function: handleEventType()
	// Description:	Identifica qual o tipo de ação realizada pelo usuário e envia a mesma para 
	//				a função específica que irá tratar de acordo.
	// Parameters:
	//		SDL_Event & event;		Contém a informação de algum ação que aconteceu efetuado pelo usuário.
	// Return: void
	// -------------------------------------------------------------
	void handleEventType(SDL_Event & event) {
		...
	}
	```

	```c++
	// -------------------------------------------------------------
	// Function: handleEvents()
	// Description: Identifica uma ação do usuário, mouse ou teclado, e chama a função 
	//				handleEventType para tratar a ação.
	// Return: void
	// -------------------------------------------------------------
	void handleEvents() {
		...
	}
	```  
	
	```c++
	// -------------------------------------------------------------
	// Function: checkIfSkip()
	// Description: Verifica se o frame foi carregado e caso contrário espera o mesmo ser carregado.
	// Return: int
	// -------------------------------------------------------------
	int checkIfSkip() {
		...
	}
	```  

	```c++
	// -------------------------------------------------------------
	// Function: checkColision()
	// Description: Realiza as verificações de se houve ou não uma colisão entre o Jack e alguma caixa.
	// Parameters:
	//		Jack * jack;				// Ponteiro para o Jack, usada para acessar as informãções do mesmo.
	//		std::vector<Box*> boxes;	// Ponteiro para as caixas existentes durante o jogo.
	// Attributes:
	//		int jackRight;				// Limite e posição x da direita do boneco Jack.
	//		int jackLeft;				// Limite e posição x da esquerda do boneco Jack.
	//		int jackTop;				// Limite e posição y da parte superior do Jack.
	//		int jackBottom;				// Limite e posição y da parte inferior do Jack.
	//		int boxRight;				// Limite e posição x da direita da caixa a ser verificada.
	//		int boxLeft;				// Limite e posição x da esquerda da caixa a ser verificada.
	//		int boxTop;					// Limite e posição y da parte superior da caixa a ser verificada.
	//		int boxBottom;				// Limite e posição y da parte inferior da caixa a ser verificada.
	// Return: bool
	// -------------------------------------------------------------
	bool checkColision(Jack * jack, std::vector<Box*> boxes) {
		...
	}
	```  

	```c++
	// -------------------------------------------------------------
	// Function: isGameFinished()
	// Description: Verifica se o jogodor requisitou o fechamento do jogo.
	// Return: bool
	// -------------------------------------------------------------
	bool isGameFinished() {
		...
	}
	```  

	```c++
	// -------------------------------------------------------------
	// Function: isLevelFinished()
	// Description:	Verifica se o jogador terminou o nível momentâneo.
	// Return: bool
	// -------------------------------------------------------------
	bool isLevelFinished() {
		...
	}
	```  

### ATRIBUTTES:
	```c++
	SDL_Surface * screen;					// Screen principal onde serão mostradas os elementos gráficos.
	SDL_Event event;						// Guarda a ação do usuário caso ela exista.
	Jack * jack;							// Ponteiro para o boneco Jack guardando suas informações.
	Level * level;							// Contém informações sobre o nível em que o usuário está jogando.
	Timer frameTime;						// Controla o funcionamento de tempo e carregamento dos frames.
	ScoreScreen * score;					// Centraliza as informações da pontuação do jogo.
	InitScreen * initScreen;				// Guarda as informações da tela inicial.
	InitScreen * wonScreen;					// Controla a tela de jogo vencido executada ao final dos níveis.
	PauseScreen * pauseScreen;				// Controla a tela de pause quando está é executada pelo usuário.
	GameOverScreen * gameOverScreen;		// Controla a tela de game over executada ao final dos níveis.
	OptionsScreen * optionsScreen;			// Controla a tela de opções.
	Label * labelPlay;						// Botão responsável por dar Play no jogo.
	Label * labelOptions;					// Botão responsável por abrir o menu de opções.
	Label * labelQuit;						// Botão que finaliza o jogo ou cancela a execução de algum nível.
	Label * labelMute;						// Botão da tela de opções que permite ou não a execução do áudio.
	Label * labelLoad;						// Botão da tela de opções e que carrega um novo jogo.
	Label * labelBack;						// Botão da tela de opções que volta para a tela inicial.
	float FRAME_MILISECOND;					// Contém os milisegundos de transição entre um frame e outro.
	bool quitGame;							// Informação se o usuário deseja sair ou não do jogo.
	bool quitLevel;							// Informação se é necessário sair ou não do nível.
	bool pauseLevel;						// Informação se o jogo está pausado ou não.
	bool gameOver;							// Informação se o jogador perdeu ou não o jogo.
	bool gameWon;							// Informação se o jogador ganhou ou não o jogo.
	int linesDeleted;						// Quantidade de linhas que já foram completadas pelo jogador.
	int maxLevelLines;						// Quantidade necessária de linhas que é preciso para o 
											// usuário ganhar o jogo.
	int actualLevel;						// Contém o número do nível em que o jogador está no momento.
	```  

### CONST:
	```c++
	static const int SCREEN_WIDTH = 854;		// Tamanho em largura da tela do jogo.
	static const int SCREEN_HEIGHT = 480;		// Tamanho em altura da tela do jogo.
	static const int SCREEN_BPP = 32;			// Número de bit por pixel permitido na tela.
	static const int SCREEN_FPS = 60;			// Quantidade de frames permitidos por segundo.
	```  
