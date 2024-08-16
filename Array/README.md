# Functions for working with arrays  

The array elemnts are supposed to be complex data types with structures and pointers to memories of other structures and so on.  

-
Strategy: These functions explicitly need to know the type of data structures they are operating on; So I'll use a character string to keep the description of the data structure and pass it into the function each time it is called.  

-  

* Generation of an array.  
```C

    void* genArray(char *dataStrctrDscrpn, int arrSize);
```  
Function that allocates memory and defines the array elements for the daughter memory blocks and variables(for complex data types).   

* Insertion of an array element  
```

    void insertArrElmnt(char *dataStrctrDscrpn ,int insertPsn);
```  
    Adds an element at a specific of the array  

* Deletion of an array element
```
    void deleteArrElmnt(char *dataStrctrDscrpn, int delPsn);
```  
    will use a function that could crawl through a data structure and free each dynamically allocated memory block associated with it.  
    This will be used to delete an element at a specific position and shift the remaining elements leftwards.  

* Searching  
```

    int searchArr(char *dataStrctrDscrpn, );
```  
    Scans through the array, as well as through the data structure of the elements, looking for a specific item, and then returns the index of the element the item belongs to.  

* Sorting
```

    void *sortArr(char *dataStrctrDscrpn,char* elementLocnInDS);
```  
    Sorts the array on the basis of an element that is numerically comparable.  

* Merging
```
    
    void *mergeArr(void *Arr1, void *Arr2);
```  
    Combines two arrays into one.

* Reversing
```

    void *reverseArr(void *Arr);
```  
    Reverses the order of elements of an array.  

* Rotating
```
    void *rotateArr(void *Arr);
```  
    Rotatates the array elements to the right or left by a certain number of positions


