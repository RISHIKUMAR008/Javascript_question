// function to find the prefix sum array
function prefSum(arr) {
    let n = arr.length;
    
    // to store the prefix sum
    let prefixSum = new Array(n);

    // initialize the first element
    prefixSum[0] = arr[0];

    // Adding present element with previous element
    for (let i = 1; i < n; i++)
        prefixSum[i] = prefixSum[i - 1] + arr[i];
    
    return prefixSum;
}

// Driver Code
let arr = [10, 20, 10, 5, 15];
let prefixSum = prefSum(arr);
for (let i of prefixSum) {
    process.stdout.write(i + " ");
}
