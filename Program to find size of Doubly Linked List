class Node {
    constructor(val) {
        this.data = val;
        this.next = null;
        this.prev = null;
    }
}

// This function returns the size
// of the linked list
function findSize(curr) {
    let size = 0;
    while (curr !== null) {
        size++;
        curr = curr.next;
    }
    return size;
}

// Create a hard-coded doubly linked list:
// 1 <-> 2 <-> 3 <-> 4
let head = new Node(1);
head.next = new Node(2);
head.next.prev = head;
head.next.next = new Node(3);
head.next.next.prev = head.next;
head.next.next.next = new Node(4);
head.next.next.next.prev = head.next.next;

console.log(findSize(head));
