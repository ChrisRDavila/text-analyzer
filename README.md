Describe: wordCounter()

Test: "It should return 1 if a passage has just one word."
Code:
const text = "hello";
wordCounter(text);
Expected Output: 1

Test: "It should return 2 if a passage has two words."
Code:
const text = "hello there";
wordCounter(text);
Expected Output: 2

Test: "It should return 0 for an empty string."
Code: wordCounter("");
Expected Output: 0

Test: "It should return 0 for a string that is only spaces."
Code: wordCounter("            ");
Expected Output: 0

Test: "It should not count numbers as words."
Code: wordCounter("hi there 77 19");
Expected Output: 2

Describe: numberOfOccurenceInText()
Test: "It should return 0 occurences of a word for an empty string."
Code: const text = "";
const word = "red";
numberOfOccurrencesInText(word, text);
Expected Output: 0

Test: "It should return 1 occurrence of a word when the word and the text are the same."
Code:
const text = "red";
const word = "red";
numberOfOccurrencesInText(word, text);
Expected Output: 1

Test: "It should return 0 occurences of a word when the word and the text are different."
Code:
const text = "red";
const word = "blue";
numberOfOccurencesInText(word, text);
Expected Output: 0

Test: "It should return the number of occurences of a word."
Code:
const text = "red blue red red red green";
const word = "red";
numberOfOccurencesInText(word, text);
Expected Output: 4

"Test: "It should return a word match regardless of case."
Code:
const text = "red RED Red green Green GREEN";
const word = "Red";
numberOfOccurencesInText(word, text);
Expected Output: 3

Test: "It should return a word match regardless of punctuation."
Code:
const text = "Red! Red. I like red, green, and yellow.";
const word = "Red";
numberOfOccurenceInText(word, text);
Expected Outcome: 3

Test: "If an empty string is passed in as a word, it should return 0."
Code:
const word = "";
const = "red RED Red!";
numberOfOccurencesInText(word, text);
Expected Output: 0 

Describe: boldPassage()

Test: "It should return null if no word or text is entered."
Code:
const text = "";
const = "";
boldPassage(word, text);
Expected: null

Test: "It should return a non-matching word in a p tag."
Code
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


Describe noOffense()

Test: "should return seperated out Array provided string in parameter that returns Array split between spaces"
Code:
const text = "hi there"
word = not testing yet
Expected Outcome: [hi, there]

 Test: "should return false if none of curse words entered in string
 Code:
 const text "hi there"
 Expected outcome: false
 
 
 
 
 Test: "should return 0 if no chosen cuss words are found in string"
 Code:
 const text: "hi there"
 const word: ["zoinks", "muppet", "biffaroni" and "loopdaloop"]
 Expected outcome: 0






 //Example to test for in noOffense "zoinks, muppeteer", "biffaroni" and "loopdaloop"














*previous test route, trying something else

Test: "It should return 0 occurences of word with an empty string"
code:
const text = "";
const word = "zoinks";
onOffense(word, text);
Expected outcome: 0

Test: "It should return 1 occurence with words that are the same"
Code:
const text = "zoinks";
const word = "zoinks";
noOffense(word, text);
Expected outcome: 1

Test: "It should return 0 ocurence with word if word and text are different"
Code:
const text = "muppeteer";
const word = "zoinks";
noOffense(word, text);
expected outcome: 0

Test: "it should return the number of occurences of chosen word"
Code:
const text = "zoinks zoinks mupeteer"
const word = "zoinks"
expected outcome: 2

Test should return the number of occurences now for all chosen cuss words"
Code:
const text = "zoinks muppeteer biffaroni loopdaloop"
const words = "zoinks muppeteer biffaroni loopdaloop"
expected outcome: 4



