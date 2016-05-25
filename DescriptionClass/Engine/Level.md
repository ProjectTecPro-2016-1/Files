### CLASS: Level
Description: Class that represents a level in the game world.

### METHODS:

```c++
// -------------------------------------------------------------
// Function: Level
// Description: Class constructor
// Parameters:
//      const string& id;
//      const string& next = "";
// Return: void
// Observation: without implementation.
// -------------------------------------------------------------
Level(const string& id, const string& next = ""){
    ...
}
```

```c++
// -------------------------------------------------------------
// Function: next()
// Description: Function that returns class m_next attribute
// Return: string
// -------------------------------------------------------------
string next() const {
    ...
}
```

```c++
// -------------------------------------------------------------
// Function: finished()
// Description: Function that returns class attribute m_done attribute
// Return: bool
// -------------------------------------------------------------
bool finished() const {
    ...
}
```

```c++
// -------------------------------------------------------------
// Function: finish()
// Description: Function that sets class attribute m_done as true
// Return: void
// -------------------------------------------------------------
void finish() {
    ...
}
```

```c++
// -------------------------------------------------------------
// Function: set_next()
// Description: Function that sets a value to class attribute m_next
// Parameters:
//      const string& next;     value that the attribute in question will receive.
// Return: void
// -------------------------------------------------------------
void set_next(const string& next) {
    ...
}
```

### ATTRIBUTES:
```c++
string m_next;  // String to next level.
bool m_done;    // Boolean variable that indicates weather the level is finished or not.
```

### CONST:
```c++
```
