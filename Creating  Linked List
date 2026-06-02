// constructor to initialize a new node with data
class Node {
    constructor(new_data) {
        this.data = new_data;
        this.next = null;
    }
}

// Create the first node (head of the list)
let head = new Node(10);

// Link the second node
head.next = new Node(20);

// Link the third node
head.next.next = new Node(30);

// Link the fourth node
head.next.next.next = new Node(40);

// printing linked list
let temp = head;
while (temp !== null) {
    process.stdout.write(temp.data + " ");
    temp = temp.next;
}
