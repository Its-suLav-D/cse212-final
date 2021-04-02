```
    class LinkedList:
        def __init__(self,value):
            self.value = value
            self.next = None

    class RemoveDuplicates(list):

    current_node = list
    while current_node is not None:
        next_node = current_node.next
        while next_node is not None and next_node.value == current_node.value:
            next_node = next_node.next

        current_node.next = next_node
        current_node = next_node
    return list

```
