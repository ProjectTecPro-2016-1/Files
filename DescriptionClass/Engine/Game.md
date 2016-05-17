## CLASS: Game
Description: Class that represents a game that will be using the engine.

### METHODS:

```c++
// -------------------------------------------------------------
// Function:
// Description:
// Parameters:
// Attributes:
// Return:
// -------------------------------------------------------------
Game(const string& id){
    ...
}
```

```c++
// -------------------------------------------------------------
// Function:
// Description:
// Parameters:
// Attributes:
// Return:
// -------------------------------------------------------------
virtual ~Game(){
    ...
}
```

```c++
// -------------------------------------------------------------
// Function: init()
// Description:
// Parameters:
//      const string & title;
//      int w;
//      int h;
//      double scale = 1.0;
//      bool fullscreen = false;
//      int volume = 50;
// Attributes:
// Return:
// -------------------------------------------------------------
void init(const string & title, int w, int h, double scale = 1.0, bool fullscreen = false,
          int volume = 50) throw (Exception){
    ...
}
```

```c++
// -------------------------------------------------------------
// Function:
// Description:
// Parameters:
// Attributes:
// Return:
// -------------------------------------------------------------
void init(const string& settings) throw (Exception){
    ...
}
```

```c++
// -------------------------------------------------------------
// Function:
// Description:
// Parameters:
// Attributes:
// Return:
// -------------------------------------------------------------
void run(){
    ...
}
```

```c++
// -------------------------------------------------------------
// Function:
// Description:
// Parameters:
// Attributes:
// Return:
// -------------------------------------------------------------
void process_input(){
    ...
}
```

```c++
// -------------------------------------------------------------
// Function:
// Description:
// Parameters:
// Attributes:
// Return:
// -------------------------------------------------------------
void update_screen(){
    ...
}
```

```c++
// -------------------------------------------------------------
// Function:
// Description:
// Parameters:
// Attributes:
// Return:
// -------------------------------------------------------------
void delay(unsigned long ms){
    ...
}
```

```c++
// -------------------------------------------------------------
// Function:
// Description:
// Parameters:
// Attributes:
// Return:
// -------------------------------------------------------------
unsigned long update_timestep() const{
    ...
}
```

```c++
// -------------------------------------------------------------
// Function:
// Description:
// Parameters:
// Attributes:
// Return:
// -------------------------------------------------------------
bool on_event(const SystemEvent& event){
    ...
}
```

```c++
// -------------------------------------------------------------
// Function:
// Description:
// Parameters:
// Attributes:
// Return:
// -------------------------------------------------------------
bool on_event(const KeyboardEvent& event){
    ...
}
```

```c++
// -------------------------------------------------------------
// Function:
// Description:
// Parameters:
// Attributes:
// Return:
// -------------------------------------------------------------
virtual Level * load_level(const string& id){
    ...
}
```

### ATTRIBUTES:
```c++
Environment *env;   //
Level *m_level;     //
string m_id;        //
bool m_done;        //
```

### CONST:
```c++
```
