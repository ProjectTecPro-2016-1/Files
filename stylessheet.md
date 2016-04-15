# _JACK THE JANITOR_ and _ENGINE_ - WIKI

### INTRODUCTION:

* This work has 2 different projects, Jack the Janitor and Engine development on "Introduction to Eletronic Games".
* Jack The Janitor and Engine are devoloped in C++.

Jack The Janitor is a puzzle game where the player controls Jack, a school's janitor who must organize the school's warehouse. Jack can push boxes to the left or right and jump boxes.
	
Jack The Janitor -> [link repository original GITHUB](https://github.com/fgagamedev/jtj)  
Engine IJE -> [link repository original GITHUB](https://github.com/fgagamedev/IJE)

<a name="summary2"></a>
<a name="summary3"></a>
<a name="summary4"></a>
<a name="summary5"></a>
<a name="summary6"></a>
## STYLESSHEET
### SUMARY
1. [Indentation and Spacing](#head2)
2. [Comments](#head3)
3. [Attributes](#head4)
4. [Class](#head5)
5. [Methods / Functions](#head6)

<a name="head2"></a>
### 1. INDENTATION and SPACING:
###### [Summary](#summary2)

* The indentation will have 4 blank spaces or a "tab" of 4 spaces.  
* Before and after mathematic operators (`+, -, *, /, %`), logics (`&&, ||, ==, !=, <=, >=, >, <`) and assignments (`=`) is obligatory to use 1 blank space.  
* In operators of assignment `++` and `--`, not need a blank space between the attribute and the operator.  
* Before `{` and after `}` are obligatory a addiction of 1 space.  
* After openned `(` and before closed `)`, not need a blank space.  
* After the name of a method, the `()` are obligatory and not need have a separation between the name and `(`.  
* After `if`, `for`, `while` are obligatory the inclusion of 1 blank space.  

**Example:**  
```c++
if (enemy != NULL) {  
	...  
}
```
```c++
if (moveDirection % 2 == 0 && movesLeft > 0) {  
	frame++;  
	if(frame > 3) {  
		frame = 1;  
	}  
}  
```
```c++
void SDLUtil::ApplySurface(int x, int y, SDL_Surface * source, SDL_Surface * destination, SDL_Rect * clip) {  
	...  
}  
```

<a name="head3"></a>
### 2. COMMENTS:
###### [Summary](#summary3)

* All comments, without exception, will have `//` in the beginning of line and 1 clear space before the text.  
* On methods and functions, need exist a sequence of comments with informacion about function, before declaration of that. The description needs to have a explication for what this method is needed. Caso as funções tenham atributos ou parâmentros, é necessário a descrição juntamente com o cabeçalho. Quando desejado, é possível informar uma observação junto ao cabeçalho da função. 
* É necessário o comentário de "nada à fazer" em elses sem ações.  

**Example:**  
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
} playingT, * playingP;`  
```  
```c++
// -------------------------------------------------------------  
// Function: ClearPlayingSounds  
// Description: Removes all currently playing sounds.  
// Return: void
// -------------------------------------------------------------  
void ClearPlayingSounds() {  
	for (int i = 0; i < MAX_PLAYING_SOUNDS; i++) {  
		playing[i].active = 0;  
	}  
}
```  
```c++
// -------------------------------------------------------------  
// Function: ClearPlayingSounds  
// Description: Destructor of class Level.  
// Return: void
// -------------------------------------------------------------  
Level::~Level() {
    if(level != NULL) {
        SDL_FreeSurface(level);
    } else {
    	// Nothing to do
    }
}
```  

<a name="head4"></a>
### 3. ATTRIBUTES:
###### [Summary](#summary4)

* The name of the attributes will be using default camelCase and the first letter is lower  
* The name of constants or "define", will composed with all letters in upper case and will be separeted by `_` between words.   
* The simbol `*` use for pointer, is obligatory need blank spaces around.  
* If necessary the inicialization of attributes, are allowed the inicialization with creation of attribute.  
* The atribution of attribute by values, will not be done in the creation of the same.    
* Não é obrigatória a declaração da variável junto ao início da função.

**Example:**  
```c++
Game game;
```
```c++
SDL_Surface * loadedImage = NULL;
loadedImage = IMG_Load(filename.c_str());
```
```c++
#define SCORESCREEN_H
```
```c++
static const int SCORE_X_OFFSET = 506;
```

<a name="head5"></a>
### 4. CLASS:
###### [Summary](#summary5)

* There 2 types, headers (.h) e as ... (.cpp)  
* The files will have the same name of classes to facilitate the includes and indentification.   
* The nomination of the classes will be done by a default CamelCase with the first upper letter.  
* The utilization of `:` will be done with blank space in both sides of `:`.   
	
**Example:**  
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

<a name="head6"></a>
### 5. METHODS / FUNCTION:
###### [Summary](#summary6)

* The name of the methods will be using defalut CamelCase and the first letter is upper for constructors and destructors, and default camelCase with first letter lower for others methods and functions.  
* All the function need to have a comments before declaration.

**Example:**  
```c++
void DrawSelf(SDL_Surface * surface);
```
```c++
void load(const string &name);
```