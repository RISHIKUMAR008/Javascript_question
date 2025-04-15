var recoverTree = function(root) {
    let first = null, second = null, prev = null;
    let curr = root, pred = null;

    while (curr) {
        if (curr.left) {
            pred = curr.left;
            while (pred.right && pred.right !== curr) {
                pred = pred.right;
            }

            if (!pred.right) {
                pred.right = curr;
                curr = curr.left;
            } else {
                if (prev && prev.val > curr.val) {
                    if (!first) first = prev;
                    second = curr;
                }
                pred.right = null;
                prev = curr;
                curr = curr.right;
            }
        } else {
            if (prev && prev.val > curr.val) {
                if (!first) first = prev;
                second = curr;
            }
            prev = curr;
            curr = curr.right;
        }
    }

    if (first && second) {
        let temp = first.val;
        first.val = second.val;
        second.val = temp;
    }
};
