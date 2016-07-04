## CLASS: Enemy
Description: Class that describes the enemies function during the game.	 					

### METHODS:
```c++
// -------------------------------------------------------------  
// Function: Enemy()  
// Description: Enemy class builder where the initializations of the variables happen.
// Parameters:  
//		string fileName;  		Enemy landscape file name.
// Return: void  
// -------------------------------------------------------------  
Enemy(std::string filename) {
	...
}
```  

```c++
// -------------------------------------------------------------  
// Function: ~Enemy()
// Description: Enemy class destructor where the landscape image files free themselves.
// Return: void  
// -------------------------------------------------------------  
~Enemy() {
	...
}
```  

```c++
// -------------------------------------------------------------  
// Function: setSpriteClips()  
// Description: Initializes the dimensions of each picture frame and each enemy moviment.
// Return: void
// -------------------------------------------------------------  
void setSpriteClips() {
	...
}
```  

```c++
// -------------------------------------------------------------  
// Function: drawSelf()  
// Description: Selects the current motion frame and draws the enemies image in specific position
//				on the screen according to the enemy attributes.
// Parameters:
//		SDL_Surface * surface;  		Pointer for surface where the graphic component will be drawn.
// Return: void  
// -------------------------------------------------------------
void drawSelf(SDL_Surface * surface) {
	...
}
```  

```c++
// -------------------------------------------------------------  
// Function: move()  
// Description: Moves the enemy horizontally according to level dimensions.
// Return: void
// -------------------------------------------------------------  
void move() {
	...
}
```  

```c++
// -------------------------------------------------------------  
// Function: throwBox()  
// Description: Controls the enemies freedom box when the right position is achieved.
// Parameters:
//		int vector<Box*> boxes;			Vector that contains boxes it´s positions.
// Return: void
// -------------------------------------------------------------  
void throwBox(vector<Box*> boxes) {
	...
}
```  

```c++
// -------------------------------------------------------------
// Function: setFirstFrame()
// Description: Setting the enemy frame according to 
//              MoveDirection and MovesLeft, the position of 
//              enemy.
// Return: void
// -------------------------------------------------------------
void Enemy::setFirstFrame(){
	...
}
```

```c++
// -------------------------------------------------------------
// Function: setSecondFrame()
// Description: Setting the enemy frame according to 
//              MoveDirection and MovesLeft, the position of 
//              enemy.
// Return: void
// -------------------------------------------------------------
void Enemy::setSecondFrame() {
	...
}
```

```c++
// -------------------------------------------------------------
// Function: setBox()
// Description: Set the box position.
// Parameters:
//      vector<Box*> boxes         Vector of boxes.
// Return: void
// -------------------------------------------------------------
void Enemy::setBox(vector<Box*> boxes){
	...	
}
```

```c++
// -------------------------------------------------------------
// Function: setStopEnemy()
// Description: Initializes the dimensions of finishing movement 
//              to right of enemy.
// Return: void
// -------------------------------------------------------------
void Enemy::setStopEnemy() {
	...
}
```

```c++
// -------------------------------------------------------------
// Function: setStartingtRightEnemyMovement()
// Description: Initializes the dimensions of starting movement 
//              to right of enemy.
// Return: void
// -------------------------------------------------------------
void Enemy::setStartingtRightEnemyMovement() {
	...
}
```

```c++
// -------------------------------------------------------------
// Function: setContinuingRightEnemyMovement()
// Description: Initializes the dimensions of continuing 
//              movement to right of enemy.
// Return: void
// -------------------------------------------------------------
void Enemy::setContinuingRightEnemyMovement() {
	...	
}
```

```c++
// -------------------------------------------------------------
// Function: setFinishingRightEnemyMovement()
// Description: Initializes the dimensions of finishing movement
//              to right of enemy.
// Return: void
// -------------------------------------------------------------
void Enemy::setFinishingRightEnemyMovement() {
	...		
}
```

```c++
// -------------------------------------------------------------
// Function: setFinishingtLeftEnemyMovement()
// Description: Initializes the dimensions of finishing movement
//              to left of enemy.
// Return: void
// -------------------------------------------------------------
void Enemy::setFinishingLeftEnemyMovement() { 
	...		
}
```

```c++
// -------------------------------------------------------------
// Function: setContinuingtLeftEnemyMovement()
// Description: Initializes the dimensions of continuing movement
//              to left of enemy.
// Return: void
// -------------------------------------------------------------
void Enemy::setContinuingLeftEnemyMovement() {
	...
}
```

```c++
// -------------------------------------------------------------
// Function: setStartingtLeftEnemyMovement()
// Description: Initializes the dimensions of starting movement
//              to left of enemy.
// Return: void
// -------------------------------------------------------------
void Enemy::setStartingtLeftEnemyMovement() { 
	...
}
```

```c++
// -------------------------------------------------------------
// Function: setDropBox()
// Description: Initializes the dimensions of finishing movement
//              to right of enemy.
// Return: void
// -------------------------------------------------------------
void Enemy::setDropBox() {
	...	
}
```

```c++
// -------------------------------------------------------------
// Function: FirstMove()
// Description: Make a movement according to the value of 
//              MovesLeft and MoveDirection of enemy.
// Return: void
// -------------------------------------------------------------
void Enemy::FirstMove() {
	...	
}
```

```c++
// -------------------------------------------------------------
// Function: SecondMove()
// Description: Make a movement according to the value of 
//              MovesLeft and MoveDirection of enemy.
// Return: void
// -------------------------------------------------------------
void Enemy::SecondMove() {
	...	
}
```

```c++
// -------------------------------------------------------------
// Function: ThirdMove()
// Description: Make a movement according to the position of 
//              enemy on x axis.
// Return: void
// -------------------------------------------------------------
void Enemy::ThirdMove() { 
	...
}
```

```c++
// -------------------------------------------------------------
// Function: FourthMove()
// Description: Make another movement according to value of
//              position of enemy on x axis.
// Return: void
// -------------------------------------------------------------
void Enemy::FourthMove() {
	...	
}
```

```c++
// -------------------------------------------------------------
// Function: FifthMove()
// Description: Make a movement according to value of
//              MovesLeft of enemy.
// Return: void
// -------------------------------------------------------------
void Enemy::FifthMove() {
	...	
}
```

```c++
// -------------------------------------------------------------
// Function: setXPosition()
// Description: Defines the enemy position in relation to the x 
//              axis. 
// Parameters:
//      int xPosition;         Enemy posistion on x axis.
// Return: void
// -------------------------------------------------------------
void Enemy::setXPosition(int xPosition) {
	...	
}
```

```c++
// -------------------------------------------------------------
// Function: getXPosition()
// Description: Return the enemy position in relation to the x 
//              axis. 
// Return: int xPosition;   Enemy posistion on x axis.
// -------------------------------------------------------------
int Enemy::getXPosition() {
	...	
}
```

```c++
// -------------------------------------------------------------
// Function: setYPosition()
// Description: Defines the enemy position in relation to the y 
//              axis. 
// Parameters:
//      int yPosition;         Enemy posistion on y axis.
// Return: void
// -------------------------------------------------------------
void Enemy::setYPosition(int yPosition) {
	...	
}
```

```c++
// -------------------------------------------------------------
// Function: getYPosition()
// Description: Return the enemy position in relation to the y 
//              axis. 
// Return: int yPosition;   Enemy posistion on y axis.
// -------------------------------------------------------------
int Enemy::getYPosition() { 
	...
}
```

```c++
// -------------------------------------------------------------
// Function: setMovesLeft()
// Description: Defines the enemy left position. 
// Parameters:
//      int movesLeft;      Value of left position of enemy.   
// Return: void
// -------------------------------------------------------------
void Enemy::setMovesLeft(int movesLeft) { 
	...
}
```

```c++
// -------------------------------------------------------------
// Function: getMovesLeft()
// Description: Return the enemy left position. 
// Return:  int movesLeft;      Value of left position of enemy.   
// -------------------------------------------------------------
int Enemy::getMovesLeft() {
	...	
}
```

```c++
// -------------------------------------------------------------
// Function: setMoveDirection()
// Description: Defines the direction of enemy. 
// Parameters:
//      int moveDirection;      Value of direction of enemy.   
// Return: void
// -------------------------------------------------------------
void Enemy::setMoveDirection(int moveDirection) {
	...		
}
```


```c++
// -------------------------------------------------------------
// Function: getMoveDirection()
// Description: Return the enemy direction. 
// Return:  int movesDirection;      Value of direction of enemy.   
// -------------------------------------------------------------
int Enemy::getMoveDirection() { 
	...
}
```

```c++
// -------------------------------------------------------------
// Function: setFrame()
// Description: Defines defines which frame the enemy is.
// Parameters:
//      int frame;      Frame value that enemy is.  
// Return: void
// -------------------------------------------------------------
void Enemy::setFrame(int frame) {
	...	
}
```

```c++
// -------------------------------------------------------------
// Function: getFrame()
// Description: Return which frame the enemy is.
// Return:  int frame;      Frame value that enemy is.  
// -------------------------------------------------------------
int Enemy::getFrame() { 
	...
}
```

### ATTRIBUTES:
```c++
SDL_Surface * enemy;			// Pointer for enemy graphic elements.
SDL_Rect spriteClips[8];		// Contains the dimensions of each motion frame.
int frame;						// Keeps the actual frame value.
int x_position;					// Axis X position where the enemy is localizated.
int y_position;					// Axis Y position where the enemy is localizated.
int movesLeft;					// Controls the enemy movements to the right.
int moveDirection;				// Controls the movements direction horizontally.
```  

### CONST
```c++
static const int ENEMY_WIDTH = 38;		// Contains the enemies width from each position occupied on screen.
static const int ENEMY_HEIGHT = 57;		// Contain the enemies height from each position occupied on screen.
```  
