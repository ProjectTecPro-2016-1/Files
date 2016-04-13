## CLASS: Game
	Description: It's the most important class of the project. It's does all operation need to game start and run, and has control of the operations in the game.
	Observation: Main.cpp call this class.

### METHODS:
	```c++
	// -------------------------------------------------------------
	// Function: init()
	// Description: Função que inicializa os atributos do jogo e chama função para iniciar o
	//				gerencialmento das propriedades gráficas
	// Parameters: void
	// Attributes: nothing
	// Return: void
	// -------------------------------------------------------------
	void init() {
		...
	}
	```  

	```c++
	// -------------------------------------------------------------
	// Function: loop()
	// Description: Gerar o ciclo de funcionamento do jogo. É necessária para manter o controle da execução
	//				dentro de uma função.
	// Parameters: void
	// Attributes: nothing
	// Return: void
	// -------------------------------------------------------------
	void loop() {
		...
	}
	```  

	```c++
	// -------------------------------------------------------------
	// Function: shutdown()
	// Description:	Terminar a execução do jogo limpando os componentes gráficos e de áudio.
	// Return: void
	// -------------------------------------------------------------
	void shutdown() {
		...
	}
	```  

	```c++
	// -------------------------------------------------------------
	// Function: initGUI()
	// Description: Necessária para centralizar a inicialização das
	//				diretivas da interface gráfica controlada pela SDL.
	// Return: void
	// -------------------------------------------------------------
	void initGUI() {
		...
	}
	```  

	```c++
	// -------------------------------------------------------------
	// Function: closeGUI()
	// Description: Centraliza a finalização de plugins das bibliotecas
	//				do SDL de audio e interface gráfica.
	// Return: void
	// -------------------------------------------------------------
	void closeGUI() {
		...
	}
	```  

	```c++
	// -------------------------------------------------------------
	// Function: wonGameScreen()
	// Description: Monta a imagem e mostra a tela de game vencido. 
					É executada apenas quando de fato o jogo termina com vitória.
	// Attributes:
	// 		bool playButton;		Contém informação se o botão de começar novo jogo foi ou não clicado.
	//		bool quitButton;		Contém informação se o botão de sair foi clicado ou não.
	// Return: void
	// -------------------------------------------------------------
	void wonGameScreen() {
		...
	}
	```  

	```c++
	// -------------------------------------------------------------
	// Function: showOptionsScreen()
	// Description:	Monta e mostra a imagem e a tela de opções do jogo juntamente com os 
	//				botões que fazem parte da mesma.
	// Attributes:
	// 		bool muteButton;		Informação se o botão de habilitar ou 
	//								desabilitar audio do jogo foi clicado ou não.
	//		bool loadButton;		Informação se o botão de carregar um jogo salvo foi clicado ou não.
	//		bool backButton;		Informaçao se o botão de retornar a tela anterior foi clicado ou não.
	// Return: void
	// -------------------------------------------------------------
	void showOptionsScreen() {
		...
	}
	```  

	```c++
	// -------------------------------------------------------------
	// Function: gameOvering()
	// Description: Chamada quando o jogo é finalizado, quando o Jack morre.
	// Return: void
	// -------------------------------------------------------------
	void gameOvering() {
		...
	}
	```  

	```c++
	// -------------------------------------------------------------
	// Function: gameOverScreenDraw()
	// Description: Origem na função gameOvering e se destina a apresentar a tela de game over para o usuário.
	// Return: void
	// -------------------------------------------------------------
	void gameOverScreenDraw() {
		...
	}
	```  

	```c++
	// -------------------------------------------------------------
	// Function: gameOverScreenLoop()
	// Description: Gera um loop na tela de game over para esperar uma ação do jogador.
	// Attributes:
	// 		bool playButton;		Contém informação se o botão de começar um jogo foi clicado ou não.
    //		bool quitButton;		Contém informação se o botão de sair do jogo foi clicado ou não.
    //		bool optionsButton;		Contém informação se o botão para acessar o 
    //								menu de opções foi clicado ou não.
	// Return: void
	// -------------------------------------------------------------
	void gameOverScreenLoop() {
		...
	}
	```  

	```c++
	// -------------------------------------------------------------
	// Function: pausingLevel()
	// Description: Chamada quando o botão de pausar o jogo é clicado durante a execução do jogo.
	// Return: void
	// -------------------------------------------------------------
	void pausingLevel() {
		...
	}
	```  

	```c++
	// -------------------------------------------------------------
	// Function: pauseScreenDraw()
	// Description: Origem na função pausingLevel e se destina a apresentar a tela de pausa para o usuário.
	// Return: void
	// -------------------------------------------------------------
	void pauseScreenDraw() {
		...
	}
	```  

	```c++
	// -------------------------------------------------------------
	// Function: pauseScreenLoop()
	// Description: Gera um loop na tela de pausa enquanto espera uma ação do jogador.
	// Attributes: 
	// 		bool playButton;		Contém informação se o botão de retornar ao jogo foi clicado ou não.
    //		bool quitButton;		Contém informação se o botão de sair do jogo foi clicado ou não.
    //		bool optionsButton;		Contém informação se o botão para acessar o 
    //								menu de opções foi clicado ou não.
	// Return: void
	// -------------------------------------------------------------
	void pauseScreenLoop() {
		...
	}
	```  

	```c++
	// -------------------------------------------------------------
	// Function: initializingScreen()
	// Description: Incia o processo de mostrar a tela de início do jogo 
	//				juntamento com a inicialização dos áudios.
	// Return: void
	// -------------------------------------------------------------
	void initializingScreen() {
		...
	}
	```  

	```c++
	// -------------------------------------------------------------
	// Function: initScreenDraw()
	// Description: Origem na função initializingScreen e se destina a apresentar a 
	//				tela de inicio do jogo para o usuário.
	// Return: void
	// -------------------------------------------------------------
	void initScreenDraw() {
		...
	}
	```  

	```c++
	// -------------------------------------------------------------
	// Function: initScreenLoop()
	// Description: Gera um loop na tela de inicio enquanto espera uma ação do jogador.
	// Attributes:
	// 		bool playButton;		Contém informação se o botão de começar um novo jogo foi clicado ou não.
    //		bool quitButton;		Contém informação se o botão de finalizar o jogo foi clicado ou não.
    //		bool optionsButton;		Contém informação se o botão para acessar o 
    //								menu de opções foi clicado ou não.
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
	// Parameters: void
	// Attributes: nothing
	// Return: void
	// -------------------------------------------------------------
	void loadCommonResources() {
		...
	}
	```  

	```c++
	// -------------------------------------------------------------
	// Function: releaseCommonResources()
	// Description:
	// Parameters: void
	// Attributes: nothing
	// Return: void
	// -------------------------------------------------------------
	void releaseCommonResources() {
		...
	}
	```  

	```c++
	// -------------------------------------------------------------
	// Function: loadProfile()
	// Description:
	// Parameters: void
	// Attributes: nothing
	// Return: void
	// -------------------------------------------------------------
	void loadProfile() {
		...
	}
	```  

	```c++
	// -------------------------------------------------------------
	// Function: saveProfile()
	// Description:
	// Parameters: void
	// Attributes: nothing
	// Return: void
	// -------------------------------------------------------------
	void saveProfile() {
		...
	}
	```  

	```c++
	// -------------------------------------------------------------
	// Function: updateTimeStep()
	// Description:
	// Parameters: void
	// Attributes: nothing
	// Return: void
	// -------------------------------------------------------------
	void updateTimeStep() {
		...
	}
	```  

	```c++
	// -------------------------------------------------------------
	// Function: handleEventMouseButtonUp()
	// Description:
	// Parameters:
	//		SDL_Event & event;		Description
	// Attributes: nothing
	// Return: void
	// -------------------------------------------------------------
	void handleEventMouseButtonUp(SDL_Event & event) {
		...
	}
	```  

	```c++
	// -------------------------------------------------------------
	// Function: handleEventMouseButtonDown()
	// Description:
	// Parameters:
	//		SDL_Event & event;		Description
	// Attributes: nothing
	// Return: void
	// -------------------------------------------------------------
	void handleEventMouseButtonDown(SDL_Event & event) {
		...
	}
	```  

	```c++
	// -------------------------------------------------------------
	// Function: handleEventKeyDown()
	// Description:
	// Parameters:
	//		SDL_Event & event;		Description
	// Attributes: nothing
	// Return: void
	// -------------------------------------------------------------
	void handleEventKeyDown(SDL_Event & event) {
		...
	}
	```

	```c++
	// -------------------------------------------------------------
	// Function: handleEventKeyUp()
	// Description:
	// Parameters:
	//		SDL_Event & event;		Description
	// Attributes: nothing
	// Return: void
	// -------------------------------------------------------------
	void handleEventKeyUp(SDL_Event & event) {
		...
	}
	```

	```c++
	// -------------------------------------------------------------
	// Function: handleEventType()
	// Description:
	// Parameters:
	//		SDL_Event & event;		Description
	// Attributes: nothing
	// Return: void
	// -------------------------------------------------------------
	void handleEventType(SDL_Event & event) {
		...
	}
	```

	```c++
	// -------------------------------------------------------------
	// Function: handleEvents()
	// Description:
	// Parameters: void
	// Attributes: nothing
	// Return: void
	// -------------------------------------------------------------
	void handleEvents() {
		...
	}
	```

	```c++
	// -------------------------------------------------------------
	// Function: runAI()
	// Description:
	// Parameters: void
	// Attributes: nothing
	// Return: void
	// -------------------------------------------------------------
	void runAI() {
		...
	}
	```

	```c++
	// -------------------------------------------------------------
	// Function: runPhysics()
	// Description:
	// Parameters: void
	// Attributes: nothing
	// Return: void
	// -------------------------------------------------------------
	void runPhysics() {
		...
	}
	```

	```c++
	// -------------------------------------------------------------
	// Function: update()
	// Description:
	// Parameters: void
	// Attributes: nothing
	// Return: void
	// -------------------------------------------------------------
	void update() {
		...
	}
	```

	```c++
	// -------------------------------------------------------------
	// Function: recieveNetworkData()
	// Description:
	// Parameters: void
	// Attributes: nothing
	// Return: void
	// -------------------------------------------------------------
	void recieveNetworkData() {
		...
	}
	```

	```c++
	// -------------------------------------------------------------
	// Function: sendNetworkData()
	// Description:
	// Parameters: void
	// Attributes: nothing
	// Return: void
	// -------------------------------------------------------------
	void sendNetworkData() {
		...
	}
	```

	```c++
	// -------------------------------------------------------------
	// Function: draw()
	// Description:
	// Parameters: void
	// Attributes: nothing
	// Return: void
	// -------------------------------------------------------------
	void draw() {
		...
	}
	```

	```c++
	// -------------------------------------------------------------
	// Function: loadLevel()
	// Description:
	// Parameters: void
	// Attributes: nothing
	// Return: void
	// -------------------------------------------------------------
	void loadLevel() {
		...
	}
	```

	```c++
	// -------------------------------------------------------------
	// Function: releaseLevel()
	// Description:
	// Parameters: void
	// Attributes: nothing
	// Return: void
	// -------------------------------------------------------------
	void releaseLevel() {
		...
	}
	```

	```c++
	// -------------------------------------------------------------
	// Function: checkIfSkip()
	// Description:
	// Parameters: void
	// Attributes: nothing
	// Return: int
	// -------------------------------------------------------------
	int checkIfSkip() {
		...
	}
	```

	```c++
	// -------------------------------------------------------------
	// Function: isGameFinished()
	// Description:
	// Parameters: void
	// Attributes: nothing
	// Return: bool
	// -------------------------------------------------------------
	bool isGameFinished() {
		...
	}
	```

	```c++
	// -------------------------------------------------------------
	// Function: isLevelFinished()
	// Description:
	// Parameters: void
	// Attributes: nothing
	// Return: bool
	// -------------------------------------------------------------
	bool isLevelFinished() {
		...
	}
	```


### ATRIBUTTES:
	```c++
	SDL_Surface * screen;					// Description
	SDL_Event event;						// Description
	Jack * jack;							// Description
	Level * level;							// Description
	Timer frameTime;						// Description
	ScoreScreen * score;					// Description
	InitScreen * initScreen;				// Description
	InitScreen * wonScreen;					// Description
	PauseScreen * pauseScreen;				// Description
	GameOverScreen * gameOverScreen;		// Description
	OptionsScreen * optionsScreen;			// Description
	Label * labelPlay;						// Description
	Label * labelOptions;					// Description
	Label * labelQuit;						// Description
	Label * labelMute;						// Description
	Label * labelLoad;						// Description
	Label * labelBack;						// Description
	float FRAME_MILISECOND;					// Description
	bool quitGame;							// Description
	bool quitLevel;							// Description
	bool pauseLevel;						// Description
	bool gameOver;							// Description
	bool gameWon;							// Description
	int linesDeleted;						// Description
	int maxLevelLines;						// Description
	int actualLevel;						// Description
	```

### CONST:
	```c++
	static const int SCREEN_WIDTH = 854;		// Description
	static const int SCREEN_HEIGHT = 480;		// Description
	static const int SCREEN_BPP = 32;			// Description
	static const int SCREEN_FPS = 60;			// Description
	```
