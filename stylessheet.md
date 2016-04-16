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
## STYLESSHEET
### SUMARY
1. [Indentation and Spacing](#headIdentation)
2. [Blank Lines](#headBlankLines)
3. [Comments](#headComments)
4. [Header] (#headHeaders)
5. [Attributes](#headAttributes)
6. [Class](#headClass)
7. [Methods / Functions](#headMethods)
8. [Asserts] (#headAsserts)
9. [Exceptions] (#headExceptions)

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
	if(frame > 3) {  
		frame = 1;  
	}  
}  
```  

* Before `{` and after `}` are obligatory a addiction of 1 space.  
* After openned `(` and before closed `)`, not need a blank space.  
* After `if`, `for`, `while` are obligatory the inclusion of 1 blank space.  

**Example:**  
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

**Example:**  
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
* At the end of function declaration.
* Is needed a blank space after `#include` and before `#define`.
* After blocks with defined action.
* After declaration of atributtes with different types.
* After declaration of methods and functions with different types and functional similarities on '.h' file.  

<a name="headComments"></a>
### 3. COMMENTS:
###### [Summary](#summary3)

* All comments, without exception, will have `//` in the beginning of line and 1 clear space before the text.  

**Example:**  
```c++
// Looking for the first box before Jack
for (int i = jackPosX; i >= 0; i--) {
	...
}
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

<a name="headHeaders"></a>
### 4. HEADERS:
###### [Summary](#summary4)

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
The description needs to have a explanation for what this method is needed. 
In case of atributtes and parameters in functions, a description along with the header is needed. 
It's possible to infomate with the function header an observation.  
* The header will have 61 simbols of `-` at beginning and at end.  

**Example:**  
```c++
// -------------------------------------------------------------  
// Function: ClearPlayingSounds  
// Description: Removes all currently playing sounds.  
// Return: void
// -------------------------------------------------------------  
void ClearPlayingSounds() {  
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


<a name="headAttributes"></a>
### 5. ATTRIBUTES:
###### [Summary](#summary5)

* The variable declaration at beginning of the function is not required.
* The name of the attributes will be using default lower camelCase.  

**Example:**  
```c++
Game game;
```  
```c++
int boxMobileBeforeJack;
```  

* The name of constants or `#define`, will composed with all letters in upper case and will be separeted by `_` between words.  

**Example:**  
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

<a name="headMethods"></a>
### 7. METHODS / FUNCTION:
###### [Summary](#summary7)

* The name of the methods will be using defalut CamelCase and the first letter is upper for constructors and destructors, and default camelCase with first letter lower for others methods and functions.  
* All the function need to have a comments before declaration.  

**Example:**  
```c++
void DrawSelf(SDL_Surface * surface);
```
```c++
void load(const string &name);
```  

<a name="headAsserts"></a>
### 8. ASSERTS:
###### [Summary](#summary8)

<a name="headExceptions"></a>
### 9. EXCEPTIONS:
###### [Summary](#summary9)