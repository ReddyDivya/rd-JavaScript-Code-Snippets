// Original array with duplicate values
const arr = ["apple", "banana", "apple"];

// Using a Set to remove duplicates
let s = new Set(arr);  // This will create a Set with unique values
let ar2 = [...s];  // Spread the Set into a new array to get an array with unique elements

console.log(ar2); // Output: ['apple', 'banana']

// Creating a hashmap to count occurrences of each element
const hashMap = {};

// Loop through each element of the original array
arr.forEach(it => {
    // If the element exists in the hashmap, increment its count
    if(it in hashMap){
        hashMap[it]++;
    }
    // Otherwise, set the initial count to 1
    else{
        hashMap[it] = 1;
    }
});

console.log(hashMap); // Output: { apple: 2, banana: 1 }
