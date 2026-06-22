class Node {
    constructor(newData) {
        this.data = newData;
        this.next = null;
    }
}
 
function reverseList(head) {
 
    let curr = head;
    let prev = null;
    let next;
 
    // traverse all the nodes of Linked List
    while (curr !== null) {
        // store next
        next = curr.next;
 
        // reverse current node's next pointer
        curr.next = prev;
 
        // move pointers one position ahead
        prev = curr;
        curr = next;
    }
 
    return prev;
}
 
function printList(node) {
    let result = [];
    while (node !== null) {
        result.push(node.data);
        node = node.next;
    }
    console.log(result.join(" -> "));
}
 
// Driver Code

let head = new Node(1);
head.next = new Node(2);
head.next.next = new Node(3);
head.next.next.next = new Node(4);
head.next.next.next.next = new Node(5);
 
head = reverseList(head);
printList(head);
