# _JACK THE JANITOR_ and _ENGINE_ - WIKI

### INTRODUCTION:

* This work has 2 different projects, Jack the Janitor and Engine development on "Introduction to Eletronic Games".
* Jack The Janitor and Engine are devoloped in C++.

Jack The Janitor is a puzzle game where the player controls Jack, a school's janitor who must organize the school's warehouse. Jack can push boxes to the left or right and jump boxes.
	
Jack The Janitor -> [link repository original GITHUB](https://github.com/fgagamedev/jtj)  
Engine IJE -> [link repository original GITHUB](https://github.com/fgagamedev/IJE)

<a name="summary1"></a>
<a name="summary2"></a>
<a name="summary3"></a>
<a name="summary4"></a>
<a name="summary5"></a>
<a name="summary6"></a>
<a name="summary7"></a>
<a name="summary8"></a>
<a name="summary9"></a>
<a name="summary10"></a>
## STYLESSHEET
### SUMARY
1. [Indentation and Spacing](#headIdentation)
2. [Blank Lines](#headBlankLines)
3. [Comments](#headComments)
4. [Header](#headHeaders)
5. [Attributes](#headAttributes)
6. [Class](#headClass)
7. [Methods / Functions](#headMethods)
8. [Asserts](#headAsserts)
9. [Exceptions](#headExceptions)
10. [Logs](#headLogs)

<a name="headIdentation"></a>
### 1. INDENTATION and SPACING:
###### [Summary](#summary1)

* The indentation will have 4 blank spaces or a "tab" of 4 spaces.  
* A maximum allowed is 100 columns.
* Before and after mathematic operators (`+, -, *, /, %`), logics (`&&, ||, ==, !=, <=, >=, >, <`) and assignments (`=`) is obligatory to use 1 blank space.  
* In operators of assignment `++` and `--`, not need a blank space between the attribute and the operator.  

**Example:**
```c++
if (moveDirection % 2 == 0 && movesLeft > 0) {  
	frame++;  
	if (frame > 3) {  
		frame = 1;  
	}  
}  
```  

* Before `{` and after `}` are obligatory a addiction of 1 space.  
* After openned `(` and before closed `)`, not need a blank space.  
* After `if`, `for`, `while` are obligatory the inclusion of 1 blank space.  

**Examples:**
```c++
if (enemy != NULL) {  
	...  
}
```  
```c++
for (int i = 0; i < MAX_PLAYING_SOUNDS; i++) {
	playing[i].active = 0;
}
```  

* After the name of a method, the `()` are obligatory and not need have a separation between the name and `(`.

**Examples:**
```c++
void SDLUtil::applySurface(int x, int y, SDL_Surface * source, SDL_Surface * destination, SDL_Rect * clip) {  
	...  
}
```  
```c++
bool isGameFinished() {
	...
}
```  

<a name="headBlankLines"></a>
### 2. BLANK LINES:
###### [Summary](#summary2)

* Is needed a blank space at the end of function declaration.  

**Example:**
```c++
void setPosition(int x, int y) {
	...
}

int getSpeed() {
	...
}
```  

* Is needed a blank space between `#include` and `#define`.  

**Examples:**
```c++
#include "SDL/SDL_ttf.h"
#include "scorescreen.h"
#include <stdio.h>

#define MAX_PLAYING_SOUNDS 10
```  
```c++
#ifndef GAME_H_
#define GAME_H_

#include <sdlutil.h>
#include <SDL/SDL.h>
```  

* After blocks with defined action is needed a blank space.  

**Example:**
```c++
void Game::shutdown() {
    SDL_LockAudio();
    free(initScreenSound.samples);
    free(level1Sound.samples);
    free(level2Sound.samples);
    free(level3Sound.samples);
    SDL_UnlockAudio();

    closeGUI();
    return;
}
```  

* After declaration of atributtes with different types is needed a blank space.  

**Example:**
```c++
bool quitGame;
bool gameWon;

int linesDeleted;
int maxLevelLines;
int actualLevel;
```  

* Is needed a blank space after declaration of methods and functions with different types and functional similarities on '.h' file.  

**Example:**
```c++
void initGUI();
void closeGUI();

void pausingLevel();
void pauseScreenDraw();
void pauseScreenLoop();

bool isGameFinished();
bool isLevelFinished();
```  

<a name="headComments"></a>
### 3. COMMENTS:
###### [Summary](#summary3)

* All comments, without exception, will have `//` in the beginning of line and 1 clear space before the text.  
* Comments to code block, need to stay one line before the block.  

**Example:**
```c++
// Looking for the first box before Jack
for (int i = jackPosX; i >= 0; i--) {
	...
}
```  

* Comments to attributes declaration and constants, need to stay in the same line and 2 tabs after the `;`.  
* Case the comment pass from 100 coluns, the comment need to be broken for other lines and need to have the same identation.  
* If the constant describe some measure, need to have a unit of measurement in the end of comment.

**Examples:**
```c++
SDL_Surface * boxMessage;		// Is the surface that contains a "box message" about the 
								// game at the time. 
```  
```c++
SDL_Surface * gameOverScreen;		// Keeps the image that loaded.
```  
```c++
static const int LEVEL_WIDTH = 854;		// Size of width screen that will show the image level, in pixels.
```  

* The comment "// Nothing to do" is required in "else" without actions.  

**Example:**
```c++
if (level != NULL) {
	SDL_FreeSurface(level);
} else {
	// Nothing to do
}
```  

* Important comments will be write with all letter in UPPER CASE.  

**Example:**
```c++
// NOTICE THAT WHEN THE GAME RESTARTS, ANOTHER BOX IS PUSHED INTO THE ARRAY
for (unsigned int i = 0; i < level->boxes.size(); i++) {
	...
}
```  

<a name="headHeaders"></a>
### 4. HEADERS:
###### [Summary](#summary4)

* The header will have 61 simbols of `-` at beginning and at end.  
* A header with name and description of class is required above declaration of class on '.h' files.  

**Example:**
```c++
// -------------------------------------------------------------  
// 	Class: PauseScreen
//	Description: Controls whats is displayed on the screen for the player when the game is paused.
// -------------------------------------------------------------  
class PauseScreen : public GameObject {
	...
};
```  

* On methods or functions and structs, need exist a sequence of comments with information about function, before declaration of that. 
* The description needs to have a explanation for what this method is needed. 
* In case of atributtes and parameters in functions, a description along with the header is needed. 

**Examples:**
```c++
// -------------------------------------------------------------
// Function: Jack()
// Description: Jack class builder where the initializations of the variables happen.
// Parameters:
//		string filename;	Name of the file from which will be loaded Jack's image.
// Return: void
// -------------------------------------------------------------
Jack(std::string filename) {
	...
}
```  
```c++
// -------------------------------------------------------------  
// 	Struct: playingS -> playingT, * playingP  
//	Description: Structure for a currently playing sound.  
// 	Atributes:  
//		int active;  		if this sound should be played  
//		sound_p sound; 		sound data to play  
//		Uint32 position; 	current position in the sound buffer  
// -------------------------------------------------------------  
typedef struct playingS {  
	int active;  
	sound_p sound;  
	Uint32 position;  
} playingT, * playingP;
```  

* It's possible to infomate with the function header an observation.  

**Example:**
```c++
// -------------------------------------------------------------  
// Function: accelerate()  
// Description: Increase the speed of the box at the right moment.
// Return: void
// Observations:
// 		Funtion not implemented
// -------------------------------------------------------------  
void accelerate() {
	...
}
```  

<a name="headAttributes"></a>
### 5. ATTRIBUTES:
###### [Summary](#summary5)

* The variable declaration at beginning of the function is not required.
* The name of the attributes will be using default lower camelCase.  

**Examples:**
```c++
Game game;
```  
```c++
int boxMobileBeforeJack;
```  

* The name of constants or `#define`, will composed with all letters in upper case and will be separeted by `_` between words. SNAKE_CASE.  

**Examples:**
```c++
#define SCORESCREEN_H
```  
```c++
static const int SCORE_X_OFFSET = 506;
```  

* The simbol `*` use for pointer, is obligatory need blank spaces around.  

**Wrong Example:**
```c++
SDL_Surface* loadedImage = NULL;
SDL_Surface *loadedImage = NULL;
```  

**Right Example:**
```c++
SDL_Surface * loadedImage = NULL;
```  

* If necessary the inicialization of attributes, are allowed the inicialization with creation of attribute.  

**Example:**
```c++
int quantidadeDeCaixas = 0;
```  
    
<a name="headClass"></a>
### 6. CLASS:
###### [Summary](#summary6)

* There 2 types, headers (.h) e as ... (.cpp)  
* The files will have the same name of classes to facilitate the includes and indentification.   
* The nomination of the classes will be done by a default CamelCase with the first upper letter.  
* The utilization of `:` will be done with blank space in both sides of `:`.  

**Examples:**
```c++
class Jack : public GameObject {
	...  
}
```
```c++
class OptionsScreen : public GameObject {
	...
}
```

<a name="headMethods"></a>
### 7. METHODS / FUNCTION:
###### [Summary](#summary7)

* The name of the methods will be using defalut CamelCase and the first letter is upper for constructors and destructors, and default camelCase with first letter lower for others methods and functions.  
* All the function need to have a comments before declaration.  

**Examples:**
```c++
void DrawSelf(SDL_Surface * surface) {
	...
}
```
```c++
void load(const string & name) {
	...
}
```  

* Case the function have many parameters and they pass 100 coluns, the parameters need to be broken in your types for other line and obligatory to use the same identation of parameters in lines above.

**Examples:**
```c++
static void applySurface(int x, int y, SDL_Surface * source, SDL_Surface * destination,
                         SDL_Rect * clip = NULL) {
    ...
}
```  

<a name="headAsserts"></a>
### 8. ASSERTS:
###### [Summary](#summary8)

* As assertivas serão usadas em funções onde existem chamadas para os métodos da biblioteca SDL,
 que contenham retorno e que podem prejudicar a experiência do jogador durante a execução do Jack the Janitor.  
* Para o uso nas chamadas de SDL, será criado uma variável do tipo do retorno do método e com nome
 diferente do padrão utilizado no sistema. Se derá da forma `result_SDL_Function` com inicialização necessária.  
* Em casos excepcionais será possível utilizar outras variáveis, porém é necessário ser variável. Como mostra no último exemplo.  

**Examples:**
```c++
int result_SDL_Init = 0;
result_SDL_Init = SDL_Init(SDL_INIT_EVERYTHING);
assert(result_SDL_Init >= 0 && "Problem to init SDL. Impossible play the game.");
```  
```c++
int result_SDL_BlitSurface = SDL_BlitSurface(source, clip, destination, &offset);
assert(result_SDL_BlitSurface >= 0 && "Error performing the blit");
```  
```c++
this->screen = SDL_SetVideoMode(SCREEN_WIDTH, SCREEN_HEIGHT, SCREEN_BPP, SDL_HWSURFACE | SDL_DOUBLEBUF);
assert(this->screen != NULL && "Problem to set a video mode. Can't show the screen of the game.");
```  

<a name="headExceptions"></a>
### 9. EXCEPTIONS:
###### [Summary](#summary9)

* Funções que geram exceções, deverão ter em sua declaração o `throw` incluso e o tipo de exceção que pode ocorrer.  
* A preferência será por tratar a exceção no momento em que a função que gera a exceção foi chamada.  

**Example:**
```c++
void drawSelf(SDL_Surface * surface) throw (Exception) {
	...
}
```  

* O tratamento da exceção será dada da maneira mostrada no exemplo abaixo.  
* Será obrigatório o uso do `cerr` ao invés do `cout`, utilizando o padrão da biblioteca std do c++ para outputs de erro.

**Example:**
```c++
try {
	score->drawSelf(this->screen);
} catch (Exception error) {
	cerr << error.message() << endl;
}

```  

<a name="headLogs"></a>
### 10. LOGS:
###### [Summary](#summary10)

* Será utilizado a saída padrão da biblioteca std `clog`, destinada a saídas de log no console.  

**Example:**
```c++
clog << "Left limit of Jack: " << xrange + xinit << endl;
```  