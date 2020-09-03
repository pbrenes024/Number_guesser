let humanScore = 0;
let computerScore = 0;
let currentRoundNumber = 1;

// Write your code below:

let generateTarget = () => {
 return Math.floor(Math.random()* 9);
 
};

let compareGuesses = (humanGuess, computerGuess, targetGuess) => {
  const humanDifference = Math.abs(target - humanGuess);
  const computerDifference = Math.abs(target - computerGuess);
    return humanDifference <= computerDifference;
};

let updateScore = winner => {
  if (winner === 'human') {
    humanScore += 1;
  } else if (winner === 'computer') {
    computerScore += 1;
  }
};

let advanceRound = () => {
  currentRoundNumber += 1;
}
