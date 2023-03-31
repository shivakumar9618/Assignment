const arr = [2.1,4, 'HYD', 8, 6.5, 5,'AC']
const numbers = [];
const strings = [];
let floatCount = 0;

for (let i = 0; i < arr.length; i++) {
  const item = arr[i];
  if (typeof item === "number" && !Number.isNaN(item) && !Number.isInteger(item)) {
    floatCount++;
  } else if (typeof item === "number") {
    numbers.push(item);
  } else if (typeof item === "string") {
    strings.push(item);
  }
}

// Sort strings in ascending order
strings.sort();

// Print the results
console.log("Numbers:", numbers);
console.log("Strings:", strings);
console.log("Float count:", floatCount);
