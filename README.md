Describe: boldPassage()

Test: "It should return null if no word or text is entered."
Code:
const text = "";
const word = "";
boldPassage(word, text);
Expected Output: null

Test: "It should return a non-matching word in a p tag."
Code:
const word = "hello";
const text = "yo";
boldPassage(word, text);
Expected Output: <p>yo</p>

Test: "It should return a matching word in a strong tag."
Code:
const word = "hello";
const text = "hello";
boldPassage(word, text);
Expected Output: <p><strong>hello</strong></p>

Test: "It should wrap words that match in strong tags but not words that don't."
Code:
const word = "hello";
const text = "hello there";
boldPassage(word, text);
Expected Output: <p><strong>hello</strong> there</p>

Description: mostCommon()

Test: "It should list the most common words."
Code:
const word = "Hi there hey yo hi hi yay yo whoa there whoa yay.";
const text = "Hi there hey yo hi hi yay yo.";
mostCommon();
Expected Output:
hi: 3
there: 2
hey: 1
yo: 2
yay: 2
whoa: 2