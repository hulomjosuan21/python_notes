## Binary Tree

```python
class Node:
    def __init__(self, key):
        self.key = key
        self.left = None
        self.right = None

class BinaryTree:
    def __init__(self):
        self.root = None

    def insert(self, key):
        if self.root is None:
            self.root = Node(key)
        else:
            self._insert_recursive(self.root, key)

    def _insert_recursive(self, node, key):
        if key < node.key:
            if node.left is None:
                node.left = Node(key)
            else:
                self._insert_recursive(node.left, key)
        else:
            if node.right is None:
                node.right = Node(key)
            else:
                self._insert_recursive(node.right, key)

    def inorder_traversal(self, node):
        if node:
            self.inorder_traversal(node.left)
            print(node.key, end=" ")
            self.inorder_traversal(node.right)

    def preorder_traversal(self, node):
        if node:
            print(node.key, end=" ")
            self.preorder_traversal(node.left)
            self.preorder_traversal(node.right)

    def postorder_traversal(self, node):
        if node:
            self.postorder_traversal(node.left)
            self.postorder_traversal(node.right)
            print(node.key, end=" ")

# Example usage
tree = BinaryTree()
tree.insert(10)
tree.insert(5)
tree.insert(15)
tree.insert(3)
tree.insert(7)

print("Inorder Traversal:")
tree.inorder_traversal(tree.root)  # Output: 3 5 7 10 15

print("\nPreorder Traversal:")
tree.preorder_traversal(tree.root)  # Output: 10 5 3 7 15

print("\nPostorder Traversal:")
tree.postorder_traversal(tree.root)  # Output: 3 7 5 15 10
```

## Linked List

```python
class ListNode:
    def __init__(self, value):
        self.value = value
        self.next = None

class LinkedList:
    def __init__(self):
        self.head = None

    def insert_at_end(self, value):
        new_node = ListNode(value)
        if self.head is None:
            self.head = new_node
            return
        temp = self.head
        while temp.next:
            temp = temp.next
        temp.next = new_node

    def insert_at_beginning(self, value):
        new_node = ListNode(value)
        new_node.next = self.head
        self.head = new_node

    def delete(self, value):
        temp = self.head
        if temp and temp.value == value:
            self.head = temp.next
            return
        prev = None
        while temp and temp.value != value:
            prev = temp
            temp = temp.next
        if temp is None:
            return
        prev.next = temp.next

    def print_list(self):
        temp = self.head
        while temp:
            print(temp.value, end=" -> ")
            temp = temp.next
        print("None")

# Example usage
ll = LinkedList()
ll.insert_at_end(10)
ll.insert_at_end(20)
ll.insert_at_end(30)
ll.insert_at_beginning(5)
print("Linked List:")
ll.print_list()  # Output: 5 -> 10 -> 20 -> 30 -> None

ll.delete(20)
print("After deleting 20:")
ll.print_list()  # Output: 5 -> 10 -> 30 -> None
```
