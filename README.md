# CharacterChecker-Asst
const readlineSync = require('readline-sync');

// Step 1: Prompt the user for a string input
const text = readlineSync.question('Enter some text: ');

// Step 2: Prompt the user for an index number
const index = readlineSync.questionInt('Enter an index number: ');

// Step 3: Use bracket notation to access the character
// Step 4: Print out the character
if (index >= 0 && index < text.length) {
  console.log(`Character at index ${index}: ${text[index]}`);
} else {
  console.log('Invalid index. Please enter a number within the range of the text.');
}
