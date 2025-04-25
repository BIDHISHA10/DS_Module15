# Ex3 (e) Largest Element in BST
## DATE:21-3-25
## AIM:
To Write a c program to find the largest value in a Binary Search Tree.

## Algorithm
1. Initialize a pointer to the root of the BST. 
2. Move to the right child in a loop while it exists. 
3. Stop when the right child is NULL. 
4. Return the current node’s value as the largest.  

## Program:
```
/*
#include <stdio.h> 
#include <stdlib.h> 
struct node 
{ 
   int info; 
   struct node *left, *right; 
}; 
struct node *createnode(int key) 
{ 
   struct node *newnode = (struct node*)malloc(sizeof(struct node)); 
   newnode->info = key; 
   newnode->left = NULL; 
   newnode->right = NULL; 
   return(newnode); 
} 
void inorder(struct node *root) 
{ 
   if(root != NULL) 
   { 
       inorder(root->left); 
       printf(" %d ",root->info); 
       inorder(root->right); 
   } 
} 
void largest(struct node *root) 
{ 
   while (root != NULL && root->right != NULL) 
   { 
       root = root->right; 
   } 
   printf("\nLargest value is %d", root->info); 
} 
EX.NO : 3(E) 
LARGEST ELEMENT IN BST 
DATE : 
  
  
 
/* 
 * Main Function 
 */ 
int main() 
{ 
  /* Creating first Tree. */ 
   struct node *newnode = createnode(25); 
   newnode->left = createnode(17); 
   newnode->right = createnode(35); 
   newnode->left->left = createnode(13); 
   newnode->left->right = createnode(19); 
   newnode->right->left = createnode(27); 
   newnode->right->right = createnode(55); 
    
   printf("Inorder traversal of tree 1 :"); 
   inorder(newnode); 
   largest(newnode); 
    
return 0; 
} 
Developed by: GOGINENI BIDHISHA
RegisterNumber:  212223040048
*/
```

## Output:
![image](https://github.com/user-attachments/assets/3275ced3-c0b6-40f3-9c3a-d5e5939f4fde)



## Result:
Thus, the C program to find the largest value in a Binary Search Tree is implemented successfully.
