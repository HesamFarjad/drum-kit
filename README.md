<img width="1440" alt="Screenshot 2024-02-29 at 08 42 51" src="https://github.com/HesamFarjad/drum-kit/assets/81914229/6a62d604-5e76-4083-a1b9-c9de89da5d99">

This code is for a drum kit website that allows users to play drum sounds either by clicking on buttons or by pressing corresponding keys on the keyboard. Here's a breakdown of how it works:

var numberOfButton = document.querySelectorAll(".drum").length;: This line selects all elements with the class "drum" and stores their count in the variable numberOfButton.

for (var i = 0; i < numberOfButton; i++) { ... }: This loop iterates over each drum element and adds a click event listener to each one.

document.querySelectorAll(".drum")[i].addEventListener("click", function () { ... }: This line adds a click event listener to each drum element. When clicked, it triggers a function that calls makeSound() and applyAnimation() functions.

document.addEventListener("keydown", function (event) { ... }: This line adds a keydown event listener to the whole document. When a key is pressed, it triggers a function that calls makeSound() and applyAnimation() functions.

function makeSound(key) { ... }: This function takes a key parameter and plays the corresponding drum sound based on a switch statement.

function applyAnimation(key) { ... }: This function takes a key parameter, selects the corresponding drum button, adds a CSS class to simulate a pressed effect, and removes it after a short delay.
