# Playable Game: Number Guessing Game

let randomNumber = Math.floor(Math.random() * 100) + 1;
let attempts = 0;
let guess;

while (guess !== randomNumber) {
    guess = parseInt(prompt("Guess a number between 1 and 100:"));
    attempts++;

    if (guess < randomNumber) {
        alert("Too low! Try again.");
    } else if (guess > randomNumber) {
        alert("Too high! Try again.");
    } else {
        alert(`Congratulations! You've guessed the number ${randomNumber} in ${attempts} attempts.`);
    }
}
