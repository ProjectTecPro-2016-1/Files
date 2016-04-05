## CLASS: Box
	Description: Classe que descreve o funcionamento das caixas que o jogador deve escapar durante o jogo.  

### METHODS:
	```c++
	// -------------------------------------------------------------  
	// Function: Box()  
	// Description: Construtor da classe Box onde acontecem as inicializações das variáveis da classe.  
	// Parameters:  
	//		string fileName;  		Nome do arquivo da imagem de fundo da caixa.
	// Atributes: nothing
	// Return: void  
	// -------------------------------------------------------------  
	Box(std::string filename) {
		...
	}
	```  
	
	```c++
	// -------------------------------------------------------------  
	// Function: ~Box() 
	// Description: Destrutor da classe Box onde acontece a limpa dos arquivos de imagem das caixas.
	// Parameters: void
	// Atributes: nothing
	// Return: void  
	// -------------------------------------------------------------  
	~Box() {
		...
	}
	```  
	
	```c++
	// -------------------------------------------------------------  
	// Function: drawSelf()  
	// Description: Desenha a caixa em uma posição específica da tela de acordo com os atributos da caixa.
	// Parameters: 
	//		SDL_Surface *surface;		Ponteiro para a surface onde será desenhado o componente gráfico.
	// Atributes: nothing
	// Return: void  
	// ------------------------------------------------------------- 
	void drawSelf(SDL_Surface *surface) {
		...
	}
	```  
	
	```c++
	// -------------------------------------------------------------  
	// Function: getPositionX()  
	// Description: Retorna a posição no eixo X da caixa no momento.
	// Parameters: void
	// Atributes: nothing
	// Return: int  
	// -------------------------------------------------------------  
	int getPositionX() {
		...
	}
	```  
	
	```c++
	// -------------------------------------------------------------  
	// Function: getPositionY()  
	// Description: Retorna a posição no eixo Y da caixa no momento.
	// Parameters: void
	// Atributes: nothing
	// Return: int  
	// -------------------------------------------------------------  
	int getPositionY() {
		...
	}
	```  
	
	```c++
	// -------------------------------------------------------------  
	// Function: getSpeed()  
	// Description: Retorna a velocidade que a caixa se move no momento.
	// Parameters: void
	// Atributes: nothing
	// Return: int  
	// -------------------------------------------------------------  
	int getSpeed() {
		...
	}
	```  
	
	```c++
	// -------------------------------------------------------------  
	// Function: setPosition()  
	// Description: Retorna a velocidade que a caixa se move no momento.
	// Parameters:
	//		int x;			Insere o valor do eixo X da caixa no atributo que guarda essa informação.
	//		int y;  		Insere o valor do eixo Y da caixa no atributo que guarda essa informação.
	// Atributes: nothing
	// Return: void  
	// -------------------------------------------------------------  
	void setPosition(int x, int y) {
		...
	}
	```  
	
	```c++
	// -------------------------------------------------------------  
	// Function: accelerate()  
	// Description: Aumenta a velocidade da caixa no momento de queda.
	// Parameters: void
	// Atributes: nothing
	// Return: void
	// Observations:
	// 		- Função não implementada.
	// -------------------------------------------------------------  
	void accelerate() {
		...
	}
	```  
	
	```c++
	// -------------------------------------------------------------  
	// Function: fall()  
	// Description: Controla a queda da caixa durante a execução do nível do jogo.
	// Parameters:
	//		int vector<Box*> grid[12];			Vetor que contém as posições das caixas na plataforma.
	// Atributes: nothing
	// Return: void
	// -------------------------------------------------------------  
	void fall(vector<Box*> grid[12]) {
		...
	}
	```  
	
### ATTRIBUTES:
	```c++
	SDL_Surface *box;		// Ponteiro para elementos gráficos de caixas.
    float speed;			// Guarda a velocidade atual da caixa.
	bool lyingDown;			// Contém a informação de se a caixa está caindo ou não.
	int xPosition;			// Guarda a posição atual da caixa no eixo X.
	int yPosition;			// Guarda a posição atual da caixa no eixo Y.
	bool used;				// Contém a informação se a caixa já está em jogo ou não.
	```  

### CONST:
	```c++
	static const int BOX_WIDTH = 38;		// Largura em pixels de todas as caixas.
	static const int BOX_HEIGHT = 38;		// Altura em pixels de todas as caixas.
	static const int ACCELERATION = 1;		// Usada para incrementar a aceleração da caixa depois da criação de cada caixa.
    static const int MAX_SPEED = 3;			// Guarda informação sobre a velocidade máxima que a caixa pode atingir.
	```  