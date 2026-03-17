### Game : Guess The Number

# 🦀 Guessing Game in Rust

A simple, interactive command-line game built with Rust. This project was created to explore Rust's core concepts like **ownership**, **pattern matching**, and **crate management**.

## 🎮 How to Play
The computer randomly selects a secret number between **1 and 100**. Your goal is to guess it!
* If your guess is too high, it will tell you "Too Big".
* If your guess is too low, it will tell you "Too small".
* If you enter something that isn't a number, the game will ignore it and let you try again.
* Once you guess correctly, you win and the game exits.

## 🚀 Getting Started

### Prerequisites
You must have [Rust and Cargo](https://www.rust-lang.org/tools/install) installed on your machine.

### Installation & Running
1. **Clone the repository:**
   ```bash
   git clone https://github.com/jameslego-ctrl/guessing-game-in-rust.git
   cd guessing-game-in-rust```
2. **Run the application:**
    ```bash
    cargo run```

### 🛠️ Key Features & Rust Concepts Used

**This project implements several fundamental Rust features:**

- std::io: Used for handling user input from the terminal.

- External Crates: Utilizes the rand crate for random number generation.

- Shadowing: Reusing the guess variable name to convert it from a String to a u32.

- Error Handling: Instead of crashing on invalid input, the game uses a match expression on a Result type to safely continue the loop.

- Enums: Using Ordering (Less, Greater, Equal) to compare values.

### 📂 Project Structure
* `src/main.rs`: The main logic of the game.

* `Cargo.toml`: Configuration and dependency list (requires rand = "0.8.5").