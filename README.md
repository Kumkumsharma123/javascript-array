# javascript-array
function first(array, n) {
    if (n === undefined) {
        return array[0];
    } else if (n <= 0) {
        return [];
    } else {
        return array.slice(0, n);
    }
}

// Test Data
console.log(first([7, 9, 0, -2]));       // Expected Output: 7
console.log(first([], 3));               // Expected Output: []
console.log(first([7, 9, 0, -2], 3));    // Expected Output: [7, 9, 0]
console.log(first([7, 9, 0, -2], 6));    // Expected Output: [7, 9, 0, -2]
console.log(first([7, 9, 0, -2], -3));   // Expected Output: []
