# forIncubator

function removeFirstTwo(list) {
  
  // Only change code below this line
  const [a, b, ...shorterList] = list; // Change this line  
  // Only change code above this line
  return shorterList;
}

const source = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10];
const sourceWithoutFirstTwo = removeFirstTwo(source);



const stats = {
  max: 56.78,
  standard_deviation: 4.34,
  median: 34.54,
  mode: 23.87,
  min: -0.75,
  average: 35.85
};

// Only change code below this line
const half = ({max, min}) => (max + min) / 2.0; 
// Only change code above this line



const result = {
  success: ["max-length", "no-amd", "prefer-arrow-functions"],
  failure: ["no-var", "var-on-top", "linebreak"],
  skipped: ["no-extra-semi", "no-dup-keys"]
};
function makeList(arr) {
  // Only change code below this line
  const failureItems = [];
  for(let i = 0; i < arr.length; i++) {
    failureItems.push(`<li class="text-warning">${arr[i]}</li>`);
  }
  // Only change code above this line

  return failureItems;
}

const failuresList = makeList(result.failure);



// Only change code below this line
class Vegetable {
  constructor(name) {
    this.name = name;
  }
  payOff() {
    console.log("to" + this.carrot + "!");
  }
}
// Only change code above this line

const carrot = new Vegetable('carrot');
console.log(carrot.name); // Should display 'carrot'


// Only change code below this line
class Thermostat { 
  constructor(fahrenheit) {
    this._fahrenheit = fahrenheit;
  }
  get temperature() {
    return (5/9)*(this._fahrenheit-32);
  }
  set temperature(celsius) {
    return this._fahrenheit = (celsius * 9.0) / 5 + 32;
  }
}
// Only change code above this line

const thermos = new Thermostat(76); // Setting in Fahrenheit scale
let temp = thermos.temperature; // 24.44 in Celsius
thermos.temperature = 26;
temp = thermos.temperature; // 26 in Celsius



import * as stringFunctions from "./string_functions.js";
// Only change code above this line

stringFunctions.uppercaseString("hello");
stringFunctions.lowercaseString("WORLD!");

export default function subtract(x, y) {
  return x - y;
}


const makeServerRequest = new Promise((resolve, reject) => {
  // responseFromServer represents a response from a server
  let responseFromServer = true;
    
  if(responseFromServer) {
    resolve("We got the data")
    // Change this line
  } else {  
    reject("Data not received")
    // Change this line
  }
});


const makeServerRequest = new Promise((resolve, reject) => {
  // responseFromServer is set to true to represent a successful response from a server
  let responseFromServer = true;
    
  if(responseFromServer) {
    resolve("We got the data");
  } else {  
    reject("Data not received");
  }
});

makeServerRequest.then(result => {
  console.log(result);
});



const makeServerRequest = new Promise((resolve, reject) => {
  // responseFromServer is set to false to represent an unsuccessful response from a server
  let responseFromServer = false;
    
  if(responseFromServer) {
    resolve("We got the data");
  } else {  
    reject("Data not received");
  }
});

makeServerRequest.then(result => {
  console.log(result);
});

makeServerRequest.catch(error => {
  console.log(error);
});



let myString = "Hello, World!";
let myRegex = /Hello/;
let result = myRegex.test(myString); // Change this line


let waldoIsHiding = "Somewhere Waldo is hiding in this text.";
let waldoRegex = /Waldo/; // Change this line
let result = waldoRegex.test(waldoIsHiding);


let petString = "James has a pet cat.";
let petRegex = /dog|cat|bird|fish/; // Change this line
let result = petRegex.test(petString);

let myString = "freeCodeCamp";
let fccRegex = /freeCodeCamp/i; // Change this line
let result = fccRegex.test(myString);

let extractStr = "Extract the word 'coding' from this string.";
let codingRegex = /coding/; // Change this line
let result = extractStr.match(codingRegex); // Change this line


let twinkleStar = "Twinkle, twinkle, little star";
let starRegex = /Twinkle/gi; // Change this line
let result = twinkleStar.match(starRegex); // Change this line

let exampleStr = "Let's have fun with regular expressions!";
let unRegex = /.un/; // Change this line
let result = unRegex.test(exampleStr);

let quoteSample = "Beware of bugs in the above code; I have only proved it correct, not tried it.";
let vowelRegex = /[aeiou]/gi; // Change this line
let result = quoteSample.match(vowelRegex); // Change this line

let quoteSample = "The quick brown fox jumps over the lazy dog.";
let alphabetRegex = /[a-z]/gi; // Change this line
let result = quoteSample.match(alphabetRegex); // Change this line

let quoteSample = "Blueberry 3.141592653s are delicious.";
let myRegex = /[h-s2-6]/ig; // Change this line
let result = quoteSample.match(myRegex); // Change this line

let quoteSample = "3 blind mice.";
let myRegex = /[^aeiou^0-9]/gi; // Change this line
let result = quoteSample.match(myRegex); // Change this line

let difficultSpelling = "Mississippi";
let myRegex = /s+/g; // Change this line
let result = difficultSpelling.match(myRegex);

// Only change code below this line
let chewieQuote = "Aaaaaaaaaaaaaaaarrrgh!";

let chewieRegex = /Aa*/; // Change this line
// Only change code above this line

let result = chewieQuote.match(chewieRegex);


let text = "<h1>Winter is coming</h1>";
let myRegex = /<.*?>/; // it's the answer!
let result = text.match(myRegex);

let reCriminals = /C+/; // Change this line

let rickyAndCal = "Cal and Ricky both like racing.";
let calRegex = /^Cal/; // Change this line
let result = calRegex.test(rickyAndCal);

let caboose = "The last car on a train is the caboose";
let lastRegex = /caboose$/; // Change this line
let result = lastRegex.test(caboose);

let quoteSample = "The five boxing wizards jump quickly.";
let alphabetRegexV2 = /\w/g; // Change this line
let result = quoteSample.match(alphabetRegexV2).length;

let quoteSample = "The five boxing wizards jump quickly.";
let nonAlphabetRegex = /\W/g; // Change this line
let result = quoteSample.match(nonAlphabetRegex).length;

let movieName = "2001: A Space Odyssey";
let numRegex = /\d/g; // Change this line
let result = movieName.match(numRegex).length;

let movieName = "2001: A Space Odyssey";
let noNumRegex = /\D/g; // Change this line
let result = movieName.match(noNumRegex).length;

let username = "JackOfAllTrades";
let userCheck = /^[a-z][a-z]+\d*$|^[a-z]\d\d+$/i; // Change this line
let result = userCheck.test(username);

let sample = "Whitespace is important in separating words";
let countWhiteSpace = /\s/g; // Change this line
let result = sample.match(countWhiteSpace);

let sample = "Whitespace is important in separating words";
let countNonWhiteSpace = /\S/g; // Change this line
let result = sample.match(countNonWhiteSpace);

let ohStr = "Ohhh no";
let ohRegex = /Oh{3,6}\sno/; // Change this line
let result = ohRegex.test(ohStr);

let haStr = "Hazzzzah";
let haRegex = /Haz{4,}ah/; // Change this line
let result = haRegex.test(haStr);

let timStr = "Timmmmber";
let timRegex = /Tim{4}ber/; // Change this line
let result = timRegex.test(timStr);

let favWord = "favorite";
let favRegex = /favou?rite/; // Change this line
let result = favRegex.test(favWord);

let sampleWord = "astronaut";
let pwRegex = /(?=\w{6})(?=\w*\d{2})/; // Change this line
let result = pwRegex.test(sampleWord);

let myString = "Eleanor Roosevelt";
let myRegex = /(Eleanor|Franklin) (([A-Z]\.?|[A-Z][a-z]+) )?Roosevelt/; // Change this line
let result = myRegex.test(myString); // Change this line
// After passing the challenge experiment with myString and see how the grouping works

let repeatNum = "42 42 42";
let reRegex = /^(\d+) \1 \1$/; // Change this line
let result = reRegex.test(repeatNum);

let str = "one two three";
let fixRegex = /(\w+)\s(\w+)\s(\w+)/; // Change this line
let replaceText = "$3 $2 $1"; // Change this line
let result = str.replace(fixRegex, replaceText);

let hello = "   Hello, World!  ";
let wsRegex = /^\s+|\s+$/g; // Change this line
let result = hello.replace(wsRegex, ""); // Change this line

function likes (names) {
  if (names.length === 0) {
    return 'no one likes this';
  } else if (names.length === 1) {
    return `${names[0]} likes this`;
  } else if (names.length === 2) {
    return `${names[0]} and ${names[1]} like this`;
  } else if (names.length === 3) {
    return `${names[0]}, ${names[1]} and ${names[2]} like this`;
  } else if (names.length > 3) {
    return `${names[0]}, ${names[1]} and ${names.length - 2} others like this`;
  }
  }

function isIsogram(str){
    var i, j;
    str = str.toLowerCase();
    for(i = 0; i < str.length; ++i) {
      for(j = i + 1; j < str.length; ++j) {
        if(str[i] === str[j]) {
          return false;
        }
      }
    }
    return true;
 }
  console.log(isIsogram('aba'));

function tribonacci(signature, n) {
    for(let i = 0; i < n -3; i++) {
    signature.push(signature.slice(i) .reduce(( a , b) => a + b),);
    }
    return signature.slice(0, n);
    }
console.log(tribonacci([1,2,3], 10));  

function spinWords(string){
    let res = '';
    let result = string.split(' ');

    for(let i = 0; i < result.length; i++) {
        if(res)  res += ' ';
            if(result[i].length > 5) {
                 res += result[i].split('').reverse().join('');
            } else {
                res += result[i];
            }                  
    }
    return res; 
  }
  console.log(spinWords( "Hey fellow warriors" ));

function descendingOrder(n){
    return Number(n.toString().split('').sort((a,b)=> b-a).join(''));
    }

function openOrSenior(data) { 
    return  data.map(x => { if(x[0] >= 55 && x[1] > 7){return "Senior";}else{return "Open";} });
}

function persistence(num) {
   let counter = 0;

   let digits = String(num).split('');

   while(digits.length > 1) {

    let result = 1;
    for(let i =0; i < digits.length; i++) {
        result = result * digits[i];
    }

    digits = String(result).split('');
    counter++;
   }
   return counter;
}

function validatePIN(str) {
    return (/^[0-9]{4}$|^[0-9]{6}$/).test(str);
  }

function solution(str, ending){
    // TODO: complete
    return str.indexOf(ending, str.length - ending.length) !== -1;
  }

function duplicateCount(text){
    let result = 0,
        soltingObject = {};
    text.toLowerCase().split('').map(str => {
        if (!soltingObject.hasOwnProperty(str)) {
          soltingObject[str] = 0;
        } else {
          if (soltingObject[str] === 0) {
            result += 1;
          }
          soltingObject[str] = soltingObject[str] + 1;
        }
    });
    return result;
  }

let output = "Get this to show once in the freeCodeCamp console and not at all in the browser console";
console.log(output);
console.clear()

let seven = 7;
let three = "3";
console.log(seven + three);
// Only change code below this line

console.log(typeof(seven));
console.log(typeof(three));

let receivables = 10;
let payables = 8;
let netWorkingCapital = receivables - payables;
console.log(`Net working capital is: ${netWorkingCapital}`);

let myArray = [1, 2, 3];
let arraySum = myArray.reduce((previous, current) =>  previous + current);
console.log(`Sum of array values is: ${arraySum}`);

<style>
  h4 {
    text-align: center;
  }
  p {
    text-align: justify;
  }
  .links {
    margin-right: 20px;

  }
  .fullCard {
    border: 1px solid #ccc;
    border-radius: 5px;
    margin: 10px 5px;
    padding: 4px;
  }
  .cardContent {
    padding: 10px;
  }
</style>
<div class="fullCard">
  <div class="cardContent">
    <div class="cardText">
      <h4>Google</h4>
      <p>Google was founded by Larry Page and Sergey Brin while they were Ph.D. students at Stanford University.</p>
    </div>
    <div class="cardLinks">
      <a href="https://en.wikipedia.org/wiki/Larry_Page" target="_blank" class="links">Larry Page</a>
      <a href="https://en.wikipedia.org/wiki/Sergey_Brin" target="_blank" class="links">Sergey Brin</a>
    </div>
  </div>
</div>

<style>
  div {
    height: 40px;
    width: 70%;
    background: black;
    margin: 50px auto;
    border-radius: 5px;
    position: relative;
  }

  #rect {
    animation-name: rainbow;
    animation-duration: 4s;
  }

  @keyframes rainbow {
    0% {
      background-color: blue;
      top: 0px;
      left: 0px;
    }
    50% {
      background-color: green;
      top: 50px;
      left: 25px;
    }
    100% {
      background-color: yellow;
      top: 0px;
      left: -25px;
    }
  }
</style>

<div id="rect"></div>

<style>

  .balls{
    border-radius: 50%;
    background: linear-gradient(
      35deg,
      #ccffff,
      #ffcccc
    );
    position: fixed;
    width: 50px;
    height: 50px;
    margin-top: 50px;
    animation-name: bounce;
    animation-duration: 2s;
    animation-iteration-count: infinite;
  }
  #ball1 {
    left: 27%;
    animation-timing-function: cubic-bezier(0.25, 0.25, 0.75, 0.75);
  }
  #ball2 {
    left: 56%;
    animation-timing-function: ease-out;
  }

  @keyframes bounce {
    0% {
      top: 0px;
    }
    100% {
      top: 249px;
    }
  }

</style>

<div class="balls" id="ball1"></div>
<div class="balls" id="ball2"></div>
