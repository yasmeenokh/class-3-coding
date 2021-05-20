# Linked List

![linkedlist](https://media.geeksforgeeks.org/wp-content/cdn-uploads/gq/2013/03/Linkedlist.png)

**A Linked List** is a sequence of Nodes that are connected/linked to each other. The most defining feature of a Linked List is that each Node references the next Node in the link.
<hr>
## ***Type of linked list:***

![types of linkedlist](https://prepinsta.com/wp-content/uploads/2020/06/Types-of-Linked-Lists.webp)

1. Singly List : a list has one (single) reference direction to the nodes which is NEXT node.
2. Doubly List : a list has two (double) references directions to the nodes, NEXT and Prev node.
3. circular list : a list that has the final node references to the head node.
* Node : refers to single item in the linked list that holds the data.
* Head : refers to the first node in the linked list.
* Current : refers to the node currently being looked at. and when we do some operations to the linked list we define the current as the head node to ensure we start at the beginning.
* Node.next : reference to the next node. And the final element is not node rather its reference to null.

## Traversal
When traversing a linked list, you are not able to use a foreach or for loop. We depend on the Next value in each node to guide us where the next reference is pointing. The Next property is exceptionally important because it will lead us where the next node is and allow us to extract the data appropriately.

![traversal](https://image.slidesharecdn.com/pptofoperationsononewaylinklist-160321113603/95/ppt-of-operations-on-one-way-link-list-8-638.jpg?cb=1458560245)

* create a current as a pointer on the Head to guarantee that are starting from the beginning
* create while loop. This loop will still run until the current is pointing on null.
* check if the value of current is equal to the value that looking for.
* If current does not contain a value, make the current as pointer on the next node.
* Once the condition becomes true, the while loop breaks
Once the current hit the end, it means did not find the value, so return false.

### Traversal Big O
The Big O of time for Includes would be O(n). This is because, at its worse case, the node we are looking for will be the very last node in the linked list. n represents the number of nodes in the linked list.
The Big O of space for Includes would be O(1). This is because there is no additional space being used than what is already given to us with the linked list input.

## Big O (Time and Space complexity)

* ***Time Complexity:*** How much more runtime do we need as the input of the algorithm increases.
* ***Space Complexity:*** How much more memory (RAM) do we need as the input of the algorithm increases.
### We express time and space complexity using ***Big O Notation***.

![big o](https://miro.medium.com/max/550/1*leuidehqYrPSmoBRRjG8zA.png)