## CLASS: SDLUtil
	Description: Classe que desenha as imagens dos elementos em posições determinadas da tela.
	
### METHODS:
    ```c++
	// -------------------------------------------------------------  
	// Function: loadImage()  
	// Description: Carrega imagem de algum elemento para desenhar na tela.
	// Parameters:
	//		string filename;			Nome do arquivo da imagem que será desenhada no elemento.
	// Atributes: nothing
	// Return: void
	// ------------------------------------------------------------- 
	static SDL_Surface *loadImage(std::string filename) {
		...
	}
	```  
	
	```c++
	// -------------------------------------------------------------  
	// Function: applySurface()  
	// Description: Aplica de a interface de acordo com os componentes gráficos.
	// Parameters:
	//		int x;								Posição no eixo X onde o elemento será desenhado.
	//		int y;								Posição no eixo Y onde o elemento será desenhado.
	//		SDL_Surface *source;				Ponteiro para o elemento que conterá o desenho.
	//		SDL_Surface *destination;			Ponteiro para o local onde o elemento estará disposto.
	//		SDL_Rect* clip;						Não se sabe.
	// Atributes: nothing
	// Return: void
	// ------------------------------------------------------------- 
	static void applySurface(int x, int y, SDL_Surface *source, SDL_Surface *destination, SDL_Rect* clip = NULL) {
		...
	}
	```  
	
### ATTRIBUTES:

### CONST: