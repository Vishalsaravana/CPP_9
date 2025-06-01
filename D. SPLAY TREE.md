# SPLAY TREE
## PROGRAM STATEMENT:

To write the right rotate module of splay tree in CPP.

## ALGORITHM:  

1.	Start the program.
2.	Define rightRotate function: It takes a node x as input.
3.	Set y as the left child of x: Assign y = x->left.
4.	Reassign the left child of x: Set x->left = y->right.
5.	Update the right child of y: Set y->right = x.
6.	Return y: The new root after the rotation is y

## PROGRAM:
```

node *rightRotate(struct node *x)
{
node*y=x->left; x->left=y->right; y->right=x; return y;

}
 ```
## OUTPUT :
![image](https://github.com/user-attachments/assets/f7f28a6c-eb91-4536-8a79-af127a3c2b07)

## RESULT:

Thus, the C++ program to write the right rotate module of splay tree in CPP is created successfully

