## CLASS: Language
Description: Class with controls the language of the game.  

### METHODS:
```c++
// -------------------------------------------------------------  
// Function: Language()  
// Description: Constructor of class that define language of the game and languages that exist on
//              xml file
// Parameters:
//		string language;     Language selected in run of the game
// Return: void  
// -------------------------------------------------------------
Language(string language) {
    ...
}
```  

```c++
// -------------------------------------------------------------  
// Function: ~Language()  
// Description: Destructor of class that define language of the game.
// Return: void  
// -------------------------------------------------------------  
~Language() {
    ...
}
```  

```c++
// -------------------------------------------------------------  
// Function: setLanguage()  
// Description: Verify and set language for the game will started
// Parameters:
//      string language;        Language that informed in run of the game - Default is English
// Return: void  
// -------------------------------------------------------------
void setLanguage(string informedLanguage) {
	...
}
```  

```c++
// -------------------------------------------------------------  
// Function: getLanguage()  
// Description: Return language that the game are be playing
// Return: string  
// -------------------------------------------------------------
string getLanguage() {
	...
}
```  

```c++
// -------------------------------------------------------------  
// Function: getText()  
// Description: Searching and returning text of xml with selected language
// Parameters:
//      string text;        Text of needs to be searching and changing
// Return: string  
// -------------------------------------------------------------
string getText(string text) {
	...
}
```  

```c++
// -------------------------------------------------------------  
// Function: searchTextReturn()  
// Description: Searching the text finding on languages exists
// Parameters:
//      xmlDocPtr document;         Xml file that will use to search the texts
//      xmlNodePtr currentNode;     Xml tag/node that index the text find
// Return: string  
// -------------------------------------------------------------
string searchTextReturn(xmlDocPtr document, xmlNodePtr currentNode) {
	...
}
```  

```c++
// -------------------------------------------------------------  
// Function: getLocationImage()  
// Description: Searching and returning location of image in xml with selected language
// Parameters:
//      string image;       Location of iamge that needs to be changing with the select language.
// Return: string  
// -------------------------------------------------------------
string getLocationImage(string image) {
	...
}
```  

```c++
// -------------------------------------------------------------  
// Function: setLanguagesExist()  
// Description: Setting the languages exists in xml files for checking the language selected
// Return: void  
// -------------------------------------------------------------
void setLanguagesExist() {
	...
}
```  

```c++
// -------------------------------------------------------------  
// Function: getLanguagesExist()  
// Description: Getting the languages exists in xml files for checking the language selected
// Return: vector of string
// -------------------------------------------------------------
vector<string> getLanguagesExist() {
	...
}
```  

```c++
// -------------------------------------------------------------  
// Function: getSearchNode()  
// Description: Getting the languages exists in xml files for checking the language selected
// Parameters:
//      xmlDocPtr document;         Xml file that will use to search the texts
//      xmlChar * nodeSearch;       Text to need to be searched
// Return: xmlXPathObjectPtr
// -------------------------------------------------------------
xmlXPathObjectPtr getSearchNode(xmlDocPtr document, xmlChar * nodeSearch) {
	...
}
```  

```c++
// -------------------------------------------------------------  
// Function: openXmlDocument()  
// Description: Open the file xml of internationalization
// Return: xmlDocPtr
// -------------------------------------------------------------
xmlDocPtr openXmlDocument() {
	...
}
```  

```c++
// -------------------------------------------------------------  
// Function: closeXmlDocument()  
// Description: Close the xml file after are used
// Parameters:
//      xmlDocPtr document;         Xml file that will closed
// Return: void
// -------------------------------------------------------------
void closeXmlDocument(xmlDocPtr document) {
	...
}
```  


### ATTRIBUTES:
```c++
std::string language;                       // Language selected in run of the game.
std::vector<std::string> languagesExist;    // Languages that exist in xml file.
```  