# random & Ten-thousand game

### note to naming python file :
it's generally not recommended to use the same name as an existing standard library module such as random. Doing so can cause confusion and potential conflicts when importing the module or using its functionality in your code. It's best to choose a different name that is unique and descriptive for your own Python files to avoid any naming clashes.  
ex : dont name the file random.py because it is standard library module.


### linked list example :
```
class Node:
    def __init__(self, data):
        self.data = data
        self.next = None

class LinkedList:
    def __init__(self):
        self.head = None

    def append(self, data):
        new_node = Node(data)
        if self.head is None:
            self.head = new_node
        else:
            current = self.head
            while current.next:
                current = current.next
            current.next = new_node

    def find_maximum(self):
        if self.head is None:
            return None

        max_value = self.head.data
        current = self.head.next

        while current:
            if current.data > max_value:
                max_value = current.data
            current = current.next

        return max_value
```
### Ten-thousand game :
1. The game is typically played with 2 or more players, taking turns in a clockwise order.

2. Each player's turn consists of rolling six dice.

3. Players accumulate points based on the dice rolled in each turn. The following scoring rules apply:
   - A single 1 is worth 100 points.
   - A single 5 is worth 50 points.
   - Three of a kind (except for 1's) are worth 100 times the face value. For example, three 2's are worth 200 points, three 3's are worth 300 points, and so on.
   - Three 1's are worth 1000 points.

4. After each roll, the player must set aside at least one scoring die (1 or 5) to keep the points earned. They can choose to set aside more scoring dice but must set aside at least one.

5. If a player sets aside all six dice and scores with all of them, they can roll all six dice again for additional points and continue their turn. If they cannot score with any of the dice in a roll, they Farkle, losing all points earned in that turn.

6. A player can choose to stop rolling at any time and add the accumulated points to their total score. Once a player reaches a total score of 10,000 or more, the game ends.

7. The first player to reach or exceed 10,000 points is declared the winner.

These are the basic rules of the Ten-thousand game, and variations can exist depending on personal preferences or house rules.
