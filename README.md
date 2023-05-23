# Data-Structures
Data -Structures is explained in this github. 

Array

                Add     Remove
Beginning       O(n)       O(n)

End             O(1)       O(1)

Middle          O(n)       O(n)

Constant time for read/write

Linear time to add/remove at any arbitrary location



## Singly Linked List

Node Contains

    Key
    Next Pointer

Front => [] => Back

Node
    Key
    Address(next node)

Singly Linked List                          No Tail     With Tail

PushFront(Key)      Add to front            O(1)
Key TopFront(Key)   return front item       O(1)
Popfront()          remove front item       O(1)   
PushBack(Key)       add to back             O(n)        O(1)
Key TopBack()       return back item        O(n)        O(1)
PopBack()           remove back item        O(n)
Boolean Find(Key)   Is key in list?         O(n)
Erase (Key)         remove key from list    O(n)
Boolean Empty()     empty list?             O(1)
AddBefore(Node,Key) adds key before node    O(n)
AddAfter(Node,Key)  adds key after node     O(1)

    

## Douly Linked List

Node
    Key
    Next Pointer
    Prev Pointer

    Singly Linked List                          No Tail     With Tail

PushFront(Key)      Add to front            O(1)
Key TopFront(Key)   return front item       O(1)
Popfront()          remove front item       O(1)   
PushBack(Key)       add to back             O(n)        O(1)
Key TopBack()       return back item        O(n)        O(1)
PopBack()           remove back item        O(1)
Boolean Find(Key)   Is key in list?         O(n)
Erase (Key)         remove key from list    O(n)
Boolean Empty()     empty list?             O(1)
AddBefore(Node,Key) adds key before node    O(1)
AddAfter(Node,Key)  adds key after node     O(1)

## Stack

Last In First Out  LIFO

Push(Key)   =>  Adds key to Collection
Pop(Key)    =>  Returns the most recently-added key
Key Pop()   => removes and returns most recently-added key
Boolean Empty() => are there any elements?

Stack can be implemetnted with either array or a linked list
For array it has limited size
For linked list it doesnot have size limitation
Each stack operation is O(1) : Push , Pop , Top , Empty
Stacks are ocassionally known as LIFO Queues

## Queues

**Using Linked List**

First Come First Serve
First In First Out

Enqueue(Key)    :   Adds key to collection
Key Deque()     :   Removes and returns least recentlly-added key

Boolean Empty() :   Are there any elements?

Implementing through Linked List

    Enque() :   New element gets added at the back  =>  List.PushBack
    Deque() :   It removes elements from the front  =>  List.TopFront and List.PopFront

**Array Implementation**

It is difficult to add elements using list implementation

Each operation is O(1)  :   Enqueue , Dequeue , Empty


## Trees

* Empty or
* A node with 
    * a key, and
    * a list of child trees

*Node*
    *Key*
    *Children* : List of children nodes
    * parent

**Binary tree**

It has atmost 2 nodes. Value of the root node is greater than or equal to all the nodes in the left child, and less than nodes in the right child.

*Node*
    *Key*
    *left
    *right
    *parent


*Height*

If tree == nil:
    return 0
else:
    return 1 + Max(Height(tree.left) , Height(tree.right))


*Size*

If tree = nil
    return 0

return 1 + Size(tree.left) + Size(tree.right)



# Tree Traversal # 

Depth-First : We completely traverse one sub-tree before a sibling sub-tree

Breadth-first : We traverse all nodes at onelevel progressing to the next level

**Depth-Traversal**

***InOrderTraversal***

InorderTraversal(tree)
if tree = nil:
    return
InorderTraversal(tree.left)
print(tree.key)
InorderTraversal(tree.right)  

It goes through left and node and right 


***PreOrderTraversal***
InorderTraversal(tree)
if tree = nil:
    return

print(tree.key)
InorderTraversal(tree.left)
InorderTraversal(tree.right)  

It goes through node and left and right 

***PostOrderTraversal***
InorderTraversal(tree)
if tree = nil:
    return

InorderTraversal(tree.left)
InorderTraversal(tree.right)  
print(tree.key)

It goes through node and left and right 



**Breadth-First**

***LevelTraversal***

if tree = nik:
    return

Queue q
q.Enqueue(tree)

Markup :  `code()`

while not q.Empty():

    node <- q.Dequeue()
    print(node)
    if node.left != nil:
        q.Enqueue(node.left)

    if node.right != nil:
        q.Enqueue(node.right)

Markup : ```javascript
         ```
Print nodes and their left and right children and....




