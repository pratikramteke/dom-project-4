# Project 4

## Original Output Image

![Original Output Image](./original%20output%20image.png)

## Task 1: Achieve the following Output using JavaScript DOM Manipulation

![Task 1 Image](./Output/DOM%20P1%20SS.png)

## JavaScript Code:

```js
const barbarianStats = document.querySelector(
  ".clash-card__unit-stats--barbarian"
);
const archer = document.querySelector(".clash-card.archer");
const archerStats = document.querySelector(".clash-card__unit-stats--archer");
const giantStats = document.querySelector(".clash-card__unit-stats--giant");
const goblin = document.querySelector(".clash-card.goblin");
const goblinStats = document.querySelector(".clash-card__unit-stats--goblin");
const wizardStats = document.querySelector(".clash-card__unit-stats--wizard");

archer.children[2].innerText = "The Archer";
goblin.children[2].innerText = "The Goblin";

main(barbarianStats, "#ec9b3b");
main(archerStats, "#ee5487");
main(giantStats, "#f6901a");
main(goblinStats, "#82bb30");
main(wizardStats, "#4facff");

function main(troop, color) {
  troop.style.background = color;
  troop.style.color = "white";
  troop.children[2].style.color = "white";
}
```
