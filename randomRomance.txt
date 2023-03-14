//romance generator// 

// array's of words//
const greeting = ["Oh my", "Cherished", "Longing for my", "Dear", "Greetings my", "Salutations"]
const adjective = ["Darling", "Beautiful", "Beloved", "Fair", "Sweet", "Ravishing", "Gorgeous"]
const title = ["Lady", "Maiden", "Betrothed", "Wife", "Girl", "Sweet", "Darling"]
const verb = ["Kiss", "Lust", "Nuzzle", "Thrust", "Lick", "Cuddle", "Smell"]
const bodypart = ["Breast", "Thigh", "Foot", "Bosum", "Neck", "Bottom", "Belly"]

function randIndex(array) {return Math.floor(Math.random() * array.length)}

function randomRomance() {
    return(`${greeting[randIndex(greeting)]} ${adjective[randIndex(adjective)]} ${title[randIndex(title)]} 
    How I miss thee. And wish to ${verb[randIndex(verb)]} upon thine ${bodypart[randIndex(bodypart)]}`)
}
let answerBox = document.getElementById("return")
function display() {answerBox.innerHTML = randomRomance()}
let button = document.getElementById("button")

button.onclick = display

