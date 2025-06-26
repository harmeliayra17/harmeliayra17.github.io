---
title: "Blackjack Game - Web-based Card Game"
date: 2024-10-06 00:00:00 +0800
categories: [Web Project]
tags: [Blackjack, JavaScript, Game, Web Game, Card Game]
image: /assets/img/blackjack-banner.png
---

## Blackjack Game - Simple Card Game Website

**Blackjack** is a classic card game built using **JavaScript**, HTML, and CSS. The web-based version allows players to challenge a bot (dealer) with betting mechanics, card logic, and visual interactions.

The player starts with a balance of $5000 and can place a bet each round. The game follows traditional Blackjack rules—try to reach **21** without going over.

---

### 🎯 Game Features

- 💵 **Starting Money**: Begin with $5000 virtual money.
- 🃏 **Card Drawing Mechanics**: Draw cards from a shuffled 52-card deck.
- 📥 **Betting System**: Input the amount to bet before each round (minimum $100).
- 🆚 **Player vs Bot**: Compete against the bot that automatically hits until reaching 17.
- 💥 **Game Logic**: Bust, hold, draw, and win/lose evaluation.
- 🧠 **Dealer**: The bot automatically hits if its score is under 17.
- 📉 **Game Over Check**: If your money reaches $0, the game ends.

---

### 💡 Technical Highlights

- Built entirely with **vanilla JavaScript**.
- Dynamic image rendering of playing cards from `/images/cards/`.
- Modular functions: `buildCards()`, `shuffleCards()`, `distributeInitialCards()`, etc.
- Game loop includes reset, take, hold, and dealer logic.
- Real-time **DOM manipulation** for updating scores and displaying results.

---

### 🧩 Core Logic Snippets

```js
function getValueOfCard(card) {
  let value = card.split("_")[0];
  if (value === "ace") return 11;
  if (["king", "queen", "jack"].includes(value)) return 10;
  return parseInt(value);
}


function checkWinner() {
  if (mySums > 21 || mySums < botSums && botSums <= 21) {
    resultElement.textContent = "You Lose";
  } else if (botSums > 21 || mySums > botSums) {
    resultElement.textContent = "You Win";
  } else {
    resultElement.textContent = "Draw";
  }
}
```

## 📂 Source Code

👉 [View on GitHub](https://github.com/dirganoob/LAB-WEB-06-2024/tree/main/H071231079/TP_5_H071231079)

---