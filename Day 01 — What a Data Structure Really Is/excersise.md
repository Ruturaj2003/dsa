1. What is a data structure in your own words?
   My: A Data stucture is the arrangement / shape of data we create to serve specific purposes as Priority and others as a trade-off , to have a optimized desired operations.

   Gpt: A data structure is a way of arranging data in memory so that certain operations are cheap and others are expensive, based on system constraints.

2. Why do operations matter more than data?
   Operations matter more than data because , we can understand and analzye the constraints the opertions will put . the intensive/ highly used operations and less used ops . and via this information we can make descisons on designing the Data strucute . Data only give us the shape of the information or type but wont tell us more than that , maybe size aswell .

   Gpt: Data is passive. Operations consume resources. Systems fail because of operations, not data.

3. Why can’t one structure be optimal for everything?
   One struct cant be optimal for everything , because it is constraint that is enforced not logically but physically . eg : u can have easy search , but heavy write . like there are trade-oifff even if they may be mnior

   Gpt: Because making one operation cheap requires a memory layout that physically makes other operations expensive.
   Ex: - Fast random access => contigous memory => expensive insert - Fast inserts => flexible memory => slow traversal

4. What operations dominate in: (I dont know this answer or what type of answers to give )

a chat app : insert msg , delte msg ,read msg

a todo list : insert , update , delete

a cache : i donkt know

#### How to answer this type of question :

For each system ask ,

1.  Which operations happens most often?
2.  Which operation must be fast?
3.  Which operation is rare but acceptable to be slow?
4.  What odering or access pattern is required ?

GPT:
Chat App:
Dominant Operations

1.  Append msg, very freq
2.  Read msg in order, very freq
3.  Random deletion , rare
4.  Random access by index, not critical

=> Append-heavy, read-heavy, ordered traversal dominates. Deletion is rare and can be expensive.

Todo List:
Dominant Operations

1.  Read entire list , very freq
2.  Update item state, frequent
3.  Insert new item , occiaonal
4.  Delete item , occaional

=> Frequent reads and updates dominate; inserts and deletes are secondary. Order and random access both matter.

Cache
A cache exists to:

- avoid expensive re-computation or i/O
- return data fast.

Dominant Operations:

1.  Read by key , exetremly freq,
2.  Insert/Update by key , frequet
3.  Eviction , occasional but important
4.  Iteration , rare

=> Key-based reads dominate, followed by writes; eviction happes occasionally but must be controlled.

> > We dont list operations - we rank them by dominance and cost.
