### CLASS: Level
Description: Class that represents a level in the game world.

### METHODS:

```c++
Level(const string& id, const string& next = ""){
    ...
}
```

```c++
string next() const
```

```c++
bool finished() const
```

```c++
void finish();
```

```c++
void set_next(const string& next);
```

ATTRIBUTES:
string m_next;
bool m_done;
