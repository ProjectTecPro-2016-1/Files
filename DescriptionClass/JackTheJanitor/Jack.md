## CLASS: Jack
Description: Class that describes Jack's actions during the game.

### METHODS:
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
// Function: ~Jack()
// Description: Jack class destructor in which images files free themselves.
// Return: void
// -------------------------------------------------------------
~Jack() {
	...
}
```

```c++
// -------------------------------------------------------------
// Function: setLimit()
// Description:	Method that assures Jack won't pass specified limits.
// Parameters:
//		int value;		Value referent to Jack's actual position.
//		int limit1;		Limit to some of Jack's directions.
//		int range;		Range of the direction specified in limit1.
// Attributes:
//		int limit2;		Limit to opposite Jack's direction in limit1;
// Return: void
// -------------------------------------------------------------
int setLimit() {
	...
}
```

```c++
// -------------------------------------------------------------
// Function: drawSelf()
// Description: Selects the current motion frame and draws Jack's image in specific position
//				on the screen according to it's attributes.
// Parameters:
//		SDL_Surface * surface;	Pointer for surface in which graphic components will be drawn
// Return: void
// -------------------------------------------------------------
void drawSelf(SDL_Surface * surface) {
	...
}
```

```c++
// -------------------------------------------------------------
// Function: isDead()
// Description:	Return the boolean variable indicating whether Jack is dead or not.
// Return: bool
// -------------------------------------------------------------
bool isDead() {
	...
}
```

```c++
// -------------------------------------------------------------
// Function: die()
// Description:	Gives the true value to the boolean variable "dead".
// Return: void
// -------------------------------------------------------------
void die() {
	...
}
```

```c++
// -------------------------------------------------------------
// Function: setSpriteClips()
// Description: Initializes the dimensions of each picture frame and each Jack's moviment.
// Return: void
// -------------------------------------------------------------
void setSpriteClips() {
	...
}
```

```c++
// -------------------------------------------------------------
// Function: setSpriteClipsStopped()
// Description: Sets Jack image stopped.
// Return: void
// -------------------------------------------------------------
void Jack::setSpriteClipsStopped() {
	...
}
```

```c++
// -------------------------------------------------------------
// Function: setSpriteClipsOneRight()
// Description: Sets Jack image to right.
// Return: void
// -------------------------------------------------------------
void Jack::setSpriteClipsOneRight() {
	...
}
```

```c++
// -------------------------------------------------------------
// Function: setSpriteClipsSecondRight()
// Description: Sets Jack image to right.
// Return: void
// -------------------------------------------------------------
void Jack::setSpriteClipsSecondRight() {
	...
}
```

```c++
// -------------------------------------------------------------
// Function: setSpriteClipsThirdRight()
// Description: Sets Jack image to right.
// Return: void
// -------------------------------------------------------------
void Jack::setSpriteClipsThirdRight() {
	...
}
```

```c++
// -------------------------------------------------------------
// Function: setSpriteClipsJumpRight()
// Description: Sets Jack image jump to right.
// Return: void
// -------------------------------------------------------------
void Jack::setSpriteClipsJumpRight() {
	...
}
```

```c++
// -------------------------------------------------------------
// Function: setSpriteClipsOneLeft()
// Description: Sets Jack image to left.
// Return: void
// -------------------------------------------------------------
void Jack::setSpriteClipsOneLeft() {
	...
}
```

```c++
// -------------------------------------------------------------
// Function: setSpriteClipsSecondLeft()
// Description: Sets Jack image to left.
// Return: void
// -------------------------------------------------------------
void Jack::setSpriteClipsSecondLeft() {
	...
}
```

```c++
// -------------------------------------------------------------
// Function: setSpriteClipsThirdLeft()
// Description: Sets Jack image to left.
// Return: void
// -------------------------------------------------------------
void Jack::setSpriteClipsThirdLeft() {
	...
}
```

```c++
// -------------------------------------------------------------
// Function: setSpriteClipsJumpLeft()
// Description: Sets Jack image jump to left.
// Return: void
// -------------------------------------------------------------
void Jack::setSpriteClipsJumpLeft() {
	...
}
```

```c++
// -------------------------------------------------------------
// Function: move()
// Description: Method that calls setLimit() to assure Jack's won't pass screen's limits.
// Parameters:
//		int xBegin;		Limit in some of Jack's directions in X axis.
//		int xRange;		Range in X axis.
//		int yBegin;		Limit in some of Jack's directions in Y axis.
//		int yRange;		Range in Y axis.
// Return: void
// -------------------------------------------------------------
void move(int xBegin, int xRange, int yBegin, int yRange) {
	...
}
```

```c++
// -------------------------------------------------------------
// Function: pushMove()
// Description: Method that makes Jack move again after pausing.
// Parameters:
//		int v;		Variable that will make Jack walk again.
// Return: void
// -------------------------------------------------------------
void pushMove(int v) {
	...
}
```

```c++
// -------------------------------------------------------------
// Function: popMove()
// Description:	Method that stops Jack when pausing.
// Parameters:
//		int v;		Variable that will stop Jack's movement.
// Return: void
// -------------------------------------------------------------
void popMove(int v) {
	...
}
```

```c++
// -------------------------------------------------------------
// Function: jump()
// Description:	Controls the act of jumping and its consequences with respect to the maximum
//				height and possible collisions with some box.
// Parameters:
//		Level * level;		Pointer to access level class.
// Return: void
// -------------------------------------------------------------
void jump(Level * level) {
	...
}
```

```c++
// -------------------------------------------------------------
// Function: calculatesMaxJumpHeightLeft()
// Description: Calculates Jack's max jump height left.
// Parameters:
//                      Level * level;          Pointer to access level class.
// Return: int
// -------------------------------------------------------------
int Jack::calculatesMaxJumpHeightLeft(Level * level) {
	...
}
```

```c++
// -------------------------------------------------------------
// Function: calculatesMaxJumpHeightRight()
// Description: Calculates Jack's max jump height right.
// Parameters:
//                      Level * level;          Pointer to access level class.
// Return: int
// -------------------------------------------------------------
int Jack::calculatesMaxJumpHeightRight(Level * level) {
	...
}
```

```c++
// -------------------------------------------------------------
// Function: getXPosition()
// Description:	Returns the current Jack's position on the X axis.
// Return: int
// -------------------------------------------------------------
int getXPosition() {
	...
}
```

```c++
// -------------------------------------------------------------
// Function: setXPosition()
// Description: Return the Jack's position on the X axis.
// Parameters:
//      int x_position;          Insert the value of axis X of jack on the attribute that keeps the
//                                        information
// Return: void
// -------------------------------------------------------------
void Jack::setXPosition(int x_position) {
	...
}
```

```c++
// -------------------------------------------------------------
// Function: controlsMaxJump1()
// Description: Controls Jack's max jump.
// Parameters:
//                      int maxJumpHeightLeft;
//                      int maxJumpHeightRight;
// Return: void
// -------------------------------------------------------------
void Jack::controlsMaxJump1(int maxJumpHeightLeft, int maxJumpHeightRight) {
	...
}
```

```c++
// -------------------------------------------------------------
// Function: controlsMaxJump2()
// Description: Controls Jack's max jump.
// Parameters:
//                      int maxJumpHeightLeft;
//                      int maxJumpHeightRight;
// Return: void
// -------------------------------------------------------------
void Jack::controlsMaxJump1(int maxJumpHeightLeft, int maxJumpHeightRight) {
	...
}
```

```c++
// -------------------------------------------------------------
// Function: getYPosition()
// Description:	Returns the current Jack's position on the Y axis.
// Return: int
// -------------------------------------------------------------
int getYPosition() {
	...
}
```

```c++
// -------------------------------------------------------------
// Function: setYPosition()
// Description: Return the Jack's position on the Y axis.
// Parameters:
//      int y_position;          Insert the value of axis Y of jack on the attribute that keeps the
//                                        information
// Return: void
// -------------------------------------------------------------
void Jack::setYPosition(int y_position) {
	...
}
```

```c++
// -------------------------------------------------------------
// Function: getSpeed()
// Description: Return the Jack's speed.
// Return: int
// -------------------------------------------------------------
int Jack::getSpeed() {
	...
}
```

```c++
// -------------------------------------------------------------
// Function: setSpeed()
// Description: Return Jack's speed.
// Parameters:
//      int speed;
// Return: void
// -------------------------------------------------------------
void Jack::setSpeed(int speed) {
	...
}
```

```c++
// -------------------------------------------------------------
// Function: getDead()
// Description: Return dead Jack.
// Return: bool
// -------------------------------------------------------------
bool Jack::getDead() {
	...
}
```

```c++
// -------------------------------------------------------------
// Function: setDead()
// Description: Return dead Jack.
// Parameters:
//      bool dead;
// Return: void
// -------------------------------------------------------------
void Jack::setDead(bool dead) {
	...
}
```

```c++
// -------------------------------------------------------------
// Function: getVerticalSpeed()
// Description: Return vertical speed of Jack.
// Return: void
// -------------------------------------------------------------
int Jack::getVerticalSpeed() {
	...
}
```

```c++
// -------------------------------------------------------------
// Function: setVerticalSpeed()
// Description: Return vertical speed of Jack.
// Parameters:
//      int verticalSpeed;
// Return: void
// -------------------------------------------------------------
void Jack::setVerticalSpeed(int verticalSpeed) {
	...
}
```

```c++
// -------------------------------------------------------------
// Function: getJumping()
// Description: Return Jack jumping.
// Return: void
// -------------------------------------------------------------
bool Jack::getJumping() {
	...
}
```

```c++
// -------------------------------------------------------------
// Function: setJumping()
// Description: Return Jack jumping.
// Parameters:
//      bool jumping;
// Return: void
// -------------------------------------------------------------
void Jack::setJumping(bool jumping) {
	...
}
```

```c++
// -------------------------------------------------------------
// Function: getLastMove()
// Description: Return Jack's last move.
// Return: void
// -------------------------------------------------------------
int Jack::getLastMove() {
	...
}
```

```c++
// -------------------------------------------------------------
// Function: setLastMove()
// Description: Return Jack's last move.
// Parameters:
//      int lastMove;
// Return: void
// -------------------------------------------------------------
void Jack::setLastMove(int lastMove) {
	...
}
```

```c++
// -------------------------------------------------------------
// Function: getLastButOneMove()
// Description: Return Jack's last but one move.
// Return: void
// -------------------------------------------------------------
int Jack::getLastButOneMove() {
	...
}
```

```c++
// -------------------------------------------------------------
// Function: setLastButOneMove()
// Description: Return Jack's last but one move.
// Parameters:
//      int lastButOneMove;
// Return: void
// -------------------------------------------------------------
void Jack::setLastButOneMove(int lastButOneMove) {
	...
}
```

```c++
// -------------------------------------------------------------
// Function: getStrength()
// Description: Return Jack's strength.
// Return: void
// -------------------------------------------------------------
int Jack::getStrength() {
	...
}
```

```c++
// -------------------------------------------------------------
// Function: setStrength()
// Description: Return Jack's strength.
// Parameters:
//      int strength;
// Return: void
// -------------------------------------------------------------
void Jack::setStrength(int strength) {
	...
}
```

```c++
// -------------------------------------------------------------
// Function: getFrame()
// Description: Return frame of Jack.
// Return: void
// -------------------------------------------------------------
int Jack::getFrame() {
	...
}
```

```c++
// -------------------------------------------------------------
// Function: setFrame()
// Description: Return frame of Jack.
// Parameters:
//      int frame;
// Return: void
// -------------------------------------------------------------
void Jack::setFrame(int frame) {
	...
}
```

```c++
// -------------------------------------------------------------
// Function: pushBox()
// Description:
// Return: void
// Observations:
// 		Funtion not implemented
// -------------------------------------------------------------
void pushBox() {
	...
}
```

### ATRIBUTTES:
```c++
SDL_Surface * jack;			// Pointer for Jack's graphic elements.
int x_position;				// Variable that store Jack's position in X axis.
int y_position;				// Variable that store Jack's position in Y axis.
bool dead;				// Stores the information whether Jack is dead or not.
int lastMove;				// Stores Jack's last move. Used to stop Jack or make him walk again.
int lastButOneMove;			// Stores Jack's last but one move. Used to stop Jack or make him walk again.
int frame; 				// Variable for animation in drawSelf() method.
int strength;				// Stores Jack's strength to move boxes.
int speed;				// Stores Jack's actual horizontal speed.
int verticalSpeed;			// Stores Jack's actual vertical Speed.
bool jumping;				// Stores the information wheter Jack is jumping or not.
```

### CONST:
```c++
static const int ACCELERATION = 1;		// Used to increment the speed in the Y axis;
static const int JACK_WIDTH = 38;		// Jack's horizontal size.
static const int JACK_HEIGHT = 57;		// Jack's vertical size.
```
