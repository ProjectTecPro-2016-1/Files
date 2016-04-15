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
	// Description: Faz a inicialização dos recursos comuns de funcionamento do jogo, como som e áudio.
	// Return: void
	// -------------------------------------------------------------
	void loadCommonResources() {
		...
	}
	```  

	```c++
	// -------------------------------------------------------------
	// Function: releaseCommonResources()
	// Description: Faz a limpeza e liberação dos recursos comuns de funcionamento do jogo.
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
	// Description: Carrega um profile que armazena dados de um usuário específico.
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
	// Description: Salva um profile do usuário para carregar em outro momento.
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
	// Description: Carrega todas as informações referentes ao nível que o jogador está, 
	//				carregando também as imagens de cada inimigo, imagem do Jack, 
	//				quantidade de caixas que cairão durante a execução, áudios e o score.
	// Attributes:
	//		string level_1_file;		Nome do arquivo da imagem de fundo do nível 1.
	//	    string level_2_file;		Nome do arquivo da imagem de fundo do nível 2.
	//	    string level_3_file;		Nome do arquivo da imagem de fundo do nível 3.
	//	    string level_1_spec;		Nome do arquivo que contém especificações do nível 1.
	//	    string level_2_spec;		Nome do arquivo que contém especificações do nível 2.
	//	    string level_3_spec;		Nome do arquivo que contém especificações do nível 3.
	//	    string currentLevelFile;	Nome do arquivo de imagem do nível que o jogador está.
	//	    string currentLevelSpec;	Nome do arquivo de especificações do nível que o jogador está.
	//		ifstream levelFile;			Controla o arquivo de especificações do nível
    //		string numberOfLevel;		Contém o número no nível lido no levelFile.
    //		string numberOfBoxes;		Contém o número do caixas que terá no nível, lido no levelFile.
    //		string numberOfEnemies;		Comtém o número de inimigos que terá no nível, lido no levelFile.
    //		string maxLines;			Contém a quantidade necessária de linhas de caixas completas 
    //									para passar de nível, lido no levelFile.
    //		int nrBoxes;				Contém o valor inteiro provindo da variável numberOfBoxes.
    //		int nrEnemies;				Contém o valor inteiro provindo da variável numberOfEnemies.
	// Return: void
	// -------------------------------------------------------------
	void loadLevel() {
		...
	}
	```  

	```c++
	// -------------------------------------------------------------
	// Function: releaseLevel()
	// Description: Deleta o nível atual liberando memória para o próximo nível ser carregado.
	// Return: void
	// -------------------------------------------------------------
	void releaseLevel() {
		...
	}
	```  

	```c++
	// -------------------------------------------------------------
	// Function: updateTimeStep()
	// Description: Inicia um novo tempo de jogo, executado assim que algum nível termina.
	// Return: void
	// -------------------------------------------------------------
	void updateTimeStep() {
		...
	}
	```  

	```c++
	// -------------------------------------------------------------
	// Function: update()
	// Description: Executa durante o loop de duração do jogo e atualiza os atributos de controle do mesmo.
	// Return: void
	// -------------------------------------------------------------
	void update() {
		...
	}
	```  

	```c++
	// -------------------------------------------------------------
	// Function: draw()
	// Description: Concentra a criação e impressão das imagens de fundo de tela de score e do nível. 
	// Return: void
	// -------------------------------------------------------------
	void draw() {
		...
	}
	```  

	```c++
	// -------------------------------------------------------------
	// Function: runAI()
	// Description: Gera as movimentações dos inimigos e as posições que eles irão soltar as caixas.
	// Return: void
	// -------------------------------------------------------------
	void runAI() {
		...
	}
	```  

	```c++
	// -------------------------------------------------------------
	// Function: runPhysics()
	// Description: Executa a física de ações como colisões, quedas, movimentações das caixas e 
	//				movimentações dos players. 
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
