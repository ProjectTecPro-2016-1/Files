## CLASS: Enemy
	Description: Classe que descreve o funcionamento dos inimigos durante o jogo.  

### METHODS:
	```c++
	// -------------------------------------------------------------  
	// Function: Enemy()  
	// Description: Construtor da classe Enemy onde acontecem as inicializações das variáveis da classe.  
	// Parameters:  
	//		string fileName;  		Nome do arquivo da imagem de fundo do inimigo.
	// Atributes: nothing
	// Return: void  
	// -------------------------------------------------------------  
	Enemy(std::string filename) {
		...
	}
	```  
	
	```c++
	// -------------------------------------------------------------  
	// Function: ~Enemy() 
	// Description: Destrutor da classe Enemy onde acontece a limpa dos arquivos de imagem dos inimigos.
	// Parameters: void
	// Atributes: nothing
	// Return: void  
	// -------------------------------------------------------------  
    ~Enemy() {
		...
	}
	```  
	
	```c++
	// -------------------------------------------------------------  
	// Function: setSpriteClips()  
	// Description: Inicializa as dimensões de cada frame de imagem para cada tipo de movimento dos inimigos.
	// Parameters: void
	// Atributes: nothing
	// Return: void
	// -------------------------------------------------------------  
	void setSpriteClips() {
		...
	}
	```  
	
	```c++
	// -------------------------------------------------------------  
	// Function: drawSelf()  
	// Description: Seleciona o frame de imagem do movimento atual e desenha a imagem do inimigo
	//				em uma posição específica da tela de acordo com os atributos do inimigo.
	// Parameters: 
	//		SDL_Surface *surface;  		Ponteiro para a surface onde será desenhado o componente gráfico.
	// Atributes: nothing
	// Return: void  
	// ------------------------------------------------------------- 
	void drawSelf(SDL_Surface *surface) {
		...
	}
	```  
	
	```c++
	// -------------------------------------------------------------  
	// Function: move()  
	// Description: Move o inimigo em alguma direção horizontal de acordo com as dimensões do nível.
	// Parameters: void
	// Atributes: nothing
	// Return: void
	// -------------------------------------------------------------  
	void move() {
		...
	}
	```  
	
	```c++
	// -------------------------------------------------------------  
	// Function: throwBox()  
	// Description: Controla a liberação da caixa pelo inimigo quando atingida a posição correta.
	// Parameters:
	//		int vector<Box*> boxes;			Vetor que contém as caixas e suas posições correspondentes.
	// Atributes: nothing
	// Return: void
	// -------------------------------------------------------------  
    void throwBox(vector<Box*> boxes) {
		...
	}
	```  

### ATTRIBUTES:
	```c++
	SDL_Surface *enemy;				// Ponteiro para elementos gráficos de inimigos.
	SDL_Rect spriteClips[8];		// Contém as dimensões de cada frame de imagem de movimento.
	int frame;						// Guarda o valor do frame atual do movimento.
	int x_position;					// Posição no eixo X de onde o inimigo está localizado.
	int y_position;					// Posição no eixo Y de onde o inimigo está localizado.
	int movesLeft;					// Controla as movimentações do inimigo para a direita.
	int moveDirection;				// Controla a direção da movimentação no sentido horizontal.
	```  
	
### CONST
	```c++
	static const int ENEMY_WIDTH = 38;			// Contém a largura que cada inimigo ocupa na tela.
	static const int ENEMY_HEIGHT = 57;			// Contém a altura que cada inimigo ocupa na tela.
	```  