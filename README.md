
////////////////////////////////////////////////
/*   Provided Code - Please Don't Edit   */
////////////////////////////////////////////////
'use strict';

function getInput() {
    console.log("Please choose either 'rock', 'paper', or 'scissors'.")
    return prompt();
}
function randomPlay() {
    var randomNumber = Math.random();
    if (randomNumber < 0.33) {
        return "rock";
    } else if (randomNumber < 0.66) {
        return "paper";
    } else {
        return "scissors";
    }
}
////////////////////////////////////////////////
/*           Write Your Code Below            */
////////////////////////////////////////////////

function getPlayerMove(move) {
    console.log("Player Move")
    // Write an expression that operates on a variable called `move`
    // If a `move` has a value, your expression should evaluate to that value.
    // However, if `move` is not specified / is null, your expression should equal `getInput()`.
    return PlayerMove;
}

function getComputerMove(move) {
    console.log("Computer Move")
    // Write an expression that operates on a variable called `move`
    // If a `move` has a value, your expression should evaluate to that value.
    // However, if `move` is not specified / is null, your expression should equal `randomPlay()`.
    return ComputerMove;
}

function getWinner(playerMove,computerMove) {
    var winner;
    // Write code that will set winner to either 'player', 'computer', or 'tie' based on the values of playerMove and computerMove.
    // Assume that the only values playerMove and computerMove can have are 'rock', 'paper', and 'scissors'.
    // The rules of the game are that 'rock' beats 'scissors', 'scissors' beats 'paper', and 'paper' beats 'rock'.
    /* YOUR CODE HERE */
    if (playerMove === "rock" && computerMove === "scissors") {
        return "winner";
        }
        else if (playerMove === "rock" && computerMove === "paper") {
            return "loser";
        }
        else (playerMove === "rock" && computerMove === "rock") {
            return "tie";
        }
    }
    if (playerMove === "paper" && computerMove === "scissors") {
        return "loser";
    }
        else if (playerMove === "paper" && computerMove === "rock") {
            return "winner";
        }
        else (playerMove === "paper" && computerMove === "paper") {
            return "tie";
        }
      }  

    if (playerMove === "scissors" && computerMove === "rock") {
        return "loser";
    }
        else if (playerMove === "scissors" && compterMove === "paper") {
            return "winner";
        }
        else (playerMove === "scissors" && computerMove === "scissors") {
            return "tie";
        }
    }
    return winner;
}

function playToFive() {
    console.log("Let's play Rock, Paper, Scissors");
    var playerWins = 0;
    var computerWins = 0;
    // Write code that plays 'Rock, Paper, Scissors' until either the player or the computer has won five times.
    /* YOUR CODE HERE */
    var winner = "";
    while (playerWins <3 || computerWins < 3) {
        if ( winner === player) {
            playerWins++
            console.log ("Player Wins!")
            return;
        } else if (winner === compter) {
            computerWins++
            console.log ("Computer Wins");
            return;
        } else if (winner === tie) {
            console.log ("Tie")
            return;
        } else {
            console.log ("error")
            return;
        }
    }
    return [playerWins, computerWins];
    console.log ("Player Chose" + "playerMove" and "Computer chose" + "computerMove");
    console.log ("The Winner of this game is" + winner);
    console.log ("The score is" + playerWins ":" computerWins);
        if (playerWins === 3 || computerWins === 3) {
            if (playerWins === 3) {
                console.log ("You win!");
            } else {
                console.log ("You lose");
            }
        }
    return [playerWins, computerWins]

