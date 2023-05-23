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

    Queue Implementation 









