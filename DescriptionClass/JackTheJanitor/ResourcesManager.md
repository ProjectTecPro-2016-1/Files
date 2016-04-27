## CLASS: ResourcesManager
Description: Class to manager the resources.  
Observation: Class without implementation. Without .cpp.  

### METHODS:
```c++
// -------------------------------------------------------------  
// Function: ResourcesManager()  
// Description: ResourcesManager class builder.
// Return: void  
// Observation:
//		Without implementation.
// -------------------------------------------------------------  
ResourcesManager() {
	...
}
```  

```c++
// -------------------------------------------------------------  
// Function: getInstance()  
// Description: Keep instance of a pointer resource.
// Return: static ResourcesManager *
// Observation:
//		Without implementation.
// -------------------------------------------------------------  
static ResourcesManager * getInstance() {
	...
}
```  

```c++
// -------------------------------------------------------------  
// Function: getImage()  
// Description:
// Parameters:
// 		const string & name;
// Return: RawImage *
// Observation:
//		Without implementation.
// -------------------------------------------------------------  
RawImage * getImage(const string & name) {
	...
}
```  

```c++
// -------------------------------------------------------------  
// Function: release()  
// Description:
// Parameters:
// 		RawImage * image;
// Return: void  
// Observation:
//		Without implementation.
// -------------------------------------------------------------  
void release(RawImage * image) {
	...
}
```  

```c++
// -------------------------------------------------------------  
// Function: load()  
// Description:
// Parameters:
// 		const string & resourcesDescription;
// Return: void
// Observation:
//		Without implementation.
// -------------------------------------------------------------  
void load(const string & resourcesDescription) {
	...
}
```  

### ATTRIBUTES:
```c++
static ResourcesManager * instance = NULL;		// Pointer to instance resources.
class ResourcesInfo;							// Contain information of resources.
vector<ResourcesInfo*> resources;				// Vector that contains information of resources.
```  

### CONST:
