![image](https://github.com/user-attachments/assets/ea41d755-0c06-4418-b06f-aff78b1ba437)# B+ TREE
## PROGRAM STATEMENT:

To write the findParent Module of the BPlus Tree in CPP.

## ALGORITHM:  

1.	Start the program.
2.	Define the findParent function: Accept the cursor (current node) and child (the child node whose parent is to be found) as input.
3.	Base Case Check: If the cursor is a leaf node or if the first child node is a leaf, return NULL because the parent cannot be found further.
4.	Search for the Child: Loop through all child pointers of the current node (cursor). If the current child pointer matches the child node, set parent to the cursor and return it.
5.	Recursive Search: If the child is not found in the current node, recursively call findParent on each child node of the cursor to search deeper in the tree.
6.	Return Parent: If a parent is found, return the parent node; otherwise, return NULL if no parent is found.
7.	End the program.

## PROGRAM:
```
Node*BPTree::findParent(Node*cursor, Node*child) { Node *parent ;
if (cursor->IS_LEAF || (cursor->ptr[0])->IS_LEAF){ return NULL;
}
for (int i= 0; i< cursor->size+1; i++){ if(cursor->ptr[i]==child)
{
parent = cursor; returnparent;
}
else{
parent =findParent(cursor->ptr[i], child); if (parent != NULL){
returnparent;
}
}
}
returnparent;
}
 ```
## OUTPUT :
![image](https://github.com/user-attachments/assets/f6a438ea-3457-4c34-a49e-7803c648bd86)

## RESULT:

Thus, the C++ program to write the findParent Module of the BPlus Tree in CPP is created successfully.
 

