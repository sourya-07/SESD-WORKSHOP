# 🧕 Mausi CLI

> A fun, colourful command-line tool that acts like your Indian aunt — offering life advice, checking the weather, generating bills, stalking GitHub profiles, and occasionally scolding you.

---

## ✨ Features

- 🎨 **Colourful output** — powered by `chalk`
- 🌐 **Live API integrations** — ZenQuotes, Open-Meteo (weather), GitHub
- 🎲 **Mini games** — coin toss, dice roll
- 🍽️ **Desi menu & billing** — order food and get a total
- ☕ **Cutting chai** — on demand

---

## 🚀 Setup

### Prerequisites
- [Node.js](https://nodejs.org) (v18+)
- npm

### Install & Build

```bash
# 1. Clone the repository
git clone https://github.com/sourya-07/SESD-WORKSHOP.git
cd SESD-WORKSHOP

# 2. Install dependencies
npm install

# 3. Compile TypeScript → dist/
npx tsc

# 4. (Optional) Link globally so you can use `mausi` anywhere
npm link
```

---

## 📋 Commands

| Command | Description |
|---|---|
| `mausi greet <name>` | Greets you in Marathi |
| `mausi menu batao` | Shows the food menu with prices |
| `mausi bill <action> <items...>` | Generates a bill for ordered items |
| `mausi gyan do` | Returns a random philosophical quote |
| `mausi toss` | Flips a coin (Heads / Tails) |
| `mausi roll` | Rolls a 6-sided dice |
| `mausi chai` | Serves a hot cup of tea ☕ |
| `mausi daato <name>` | Mausi scolds you 😤 |
| `mausi taarif <name>` | Mausi praises you 🥰 |
| `mausi weather <city>` | Live weather for any city |
| `mausi github <username>` | GitHub profile lookup |

---

## 💡 Examples

**Greet**
```bash
$ node dist/mausi.js greet Soury
Kasa Kaay Soury
```

**Menu**
```bash
$ node dist/mausi.js menu batao

--- MAUSI KA MENU ---
Murgh_Musallam: ₹450
Garlic_Naan: ₹150
Jeera_Rice: ₹200
Sewai: ₹250
Coke: ₹100
---------------------
```

**Bill**
```bash
$ node dist/mausi.js bill khana Murgh_Musallam Garlic_Naan Coke

--- BILL BANAYEIN ---
ITEM: Murgh_Musallam COST: ₹450
ITEM: Garlic_Naan COST: ₹150
ITEM: Coke COST: ₹100
---------------------
Total Bill: ₹700
```

**Weather**
```bash
$ node dist/mausi.js weather Delhi

Mausi kehti hai: Delhi, India
🌡️  Temperature : 22.4°C
💨  Wind Speed  : 6.2 km/h
🌤️  Condition   : Clear sky ☀️
🕰️  Time        : Raat
```

**Gyan (Quote)**
```bash
$ node dist/mausi.js gyan do

"Quality is not an act, it is a habit."
- Aristotle
```

**GitHub**
```bash
$ node dist/mausi.js github torvalds

👾 Mausi ne GitHub par dhoond nikala: torvalds
Name: Linus Torvalds
Bio: Nahi diya
Public Repos: 11
Followers: 288566
```

**Daato (Scold)**
```bash
$ node dist/mausi.js daato Rahul
Nalayak Rahul, din bhar phone mein laga rehta hai!
```

---

## 🛠️ Tech Stack

| Package | Purpose |
|---|---|
| `typescript` | Type-safe development |
| `commander` | CLI argument parsing |
| `axios` | HTTP requests |
| `chalk` | Colourful terminal output |

### APIs Used (no API key required)
| API | Used for |
|---|---|
| [ZenQuotes](https://zenquotes.io) | Random philosophical quotes |
| [Open-Meteo](https://open-meteo.com) | Live weather data |
| [GitHub REST API](https://api.github.com) | Public user profile info |

---

## 📁 Project Structure

```
SESD-WORKSHOP/
├── mausi.ts          # Main CLI source file
├── dist/             # Compiled JS output (after npx tsc)
├── package.json
├── tsconfig.json
└── README.md
```

---

*Jeete raho! 🧕*
