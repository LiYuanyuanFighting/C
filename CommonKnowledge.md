### Pointer  
[Beginner's guide](https://www.programiz.com/c-programming/c-pointers)  
1.for variable **var** in the program, &var stands for the address in the memory.  
**&** is called the reference operator, it gives you the address of a variable.  
e.g. scanf("%d", &var): used to store the user inputted value in the address of **var**. 
2. **Pointer variables(pointer)**. 
it just stores the address of another variable.   
*: dereference operator, it gets you the value from the address.  
Note: the * sign when declaring a pointer is not a dereference operator. It is just a   
similar notation that creates a pointer.  
Then take care of the following 2 examples.  

#### Access Elements of an Array Using Pointer. 
    #include <stdio.h>
    
    int main()
    {
    	int data[5], i;
    	printf("Enter elements: ");
    
    	for (i=0; i<5; ++i)
    		 scanf("%d", data+i);
    	printf("You entered: \n");
    	for (i =0; i<5; ++i)
    		printf("%d\n", *(data+i));
    
    	return 0;
    }

#### Pointer to pointer. 
When we define a pointer to a pointer, the first pointer contains the address of the second pointer, which points to the location that contains the actual value. 
When a target value is indirectly pointed to by a pointer to a pointer, accessing that value requires that the asterisk operator be applied twice. 
[detailed version](https://www.tutorialspoint.com/cprogramming/c_pointer_to_pointer.htm). 
