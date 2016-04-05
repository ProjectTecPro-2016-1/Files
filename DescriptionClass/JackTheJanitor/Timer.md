## CLASS: Timer
	Description: Classe que controla o funcionamento do tempo no jogo.  

### METHODS:
	```c++
	// -------------------------------------------------------------  
	// Function: Timer()  
	// Description: Construtor da classe Timer onde acontecem as inicializações dos atributos da classe.  
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
	// Description: Altera os atributos de status dos jogos afim de iniciar um novo jogo.  
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
	// Description: Altera os atributos de status do jogo afim de paralizar.  
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
	// Description: Altera os atributos de status do jogo afim de pausar.  
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
	// Description: Altera os atributos de status do jogo afim de tirar a pausa.  
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
	// Description: Função que gera um delay na transição em um frame e outro carregamento.
	// Parameters:
	//		float ratioFPS;  		Tempo que durará o delay.
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
	// Description: Retorna o instante do jogo atual.
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
	// Description: Retorna a informação de se o jogo está iniciado ou não.
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
	// Description: Retorna a informação de se o jogo está pausado ou não.
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
	int startTicks;			// Guarda o tempo que o jogo durou ou está durando.
	int pausedTicks;		// Guarda o tempo que o jogo durou a pausa do jogo.
	bool paused;			// Contém informação de se o jogo está pausado ou não.
	bool started;			// Contém informação de se o jogo está iniciado ou não.
	```  

### CONST: