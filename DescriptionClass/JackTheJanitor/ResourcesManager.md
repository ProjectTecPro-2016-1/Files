## CLASS: ResourcesManager
	Description: Class to manager os resources.  
	Observation: Class without implementation. Without .cpp.  

### METHODS:
	```c++
	// -------------------------------------------------------------  
	// Function: ResourcesManager()  
	// Description: ResourcesManager class builder.
	// Parameters: void
	// Atributes: nothing
	// Return: void  
	// Observation: Without implementation.
	// -------------------------------------------------------------  
	ResourcesManager() {
		...
	}
	```  
	
	```c++
	// -------------------------------------------------------------  
	// Function: getInstance()  
	// Description: Keep instance of a pointer resource.
	// Parameters: void
	// Atributes: nothing
	// Return: static ResourcesManager * 
	// Observation: Without implementation.
	// -------------------------------------------------------------  
	static ResourcesManager *getInstance() {
		...
	}
	```  
	
    ```c++
	// -------------------------------------------------------------  
	// Function: getImage()  
	// Description:
	// Parameters:
	// 		const string &name;
	// Atributes: nothing
	// Return: RawImage *
	// Observation: Without implementation.
	// -------------------------------------------------------------  
	RawImage* getImage(const string &name) {
		...
	}
	```  
	
    ```c++
	// -------------------------------------------------------------  
	// Function: release()  
	// Description:
	// Parameters:
	// 		RawImage *image;
	// Atributes: nothing
	// Return: void  
	// Observation: Without implementation.
	// -------------------------------------------------------------  
	void release(RawImage *image) {
		...
	}
	```  
	
    ```c++
	// -------------------------------------------------------------  
	// Function: load()  
	// Description:
	// Parameters:
	// 		const string &resourcesDescription;
	// Atributes: nothing
	// Return: void
	// Observation: Without implementation.	
	// -------------------------------------------------------------  
	void load(const string &resourcesDescription) {
		...
	}
	```  

### ATTRIBUTES:
    ```c++
	static ResourcesManager* instance = NULL;		// Pointer to instance resources.
	class ResourcesInfo;							// Contain information of resources.
	vector<ResourcesInfo*> resources;				// Vector that contains information of resources.
	```  

### CONST: