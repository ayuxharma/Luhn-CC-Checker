# Credit Card Validator using Luhn Algorithm

## Overview
This project is a simple C++ program that validates credit card numbers using the **Luhn Algorithm**. The program checks whether a given credit card number is valid by following the standard checksum process. It continuously prompts the user for input until they decide to exit.

## Features
- Uses the **Luhn Algorithm** to validate credit card numbers.
- Accepts numerical input from the user.
- Allows the user to exit by entering "exit".
- Handles incorrect input gracefully.

## Luhn Algorithm Explained
The **Luhn Algorithm** (also known as the Modulus 10 or mod 10 algorithm) is a simple checksum formula used to validate credit card numbers. The steps are:
1. Double every second digit from right to left. If doubling results in a two-digit number, sum both digits to get a single-digit value.
2. Add the sum of the digits obtained in Step 1 to the sum of the digits that were not doubled.
3. If the total sum is a multiple of 10, the number is **valid**; otherwise, it is **invalid**.

## How to Run the Program
### Prerequisites
- A C++ compiler (such as `g++`).
- Basic knowledge of running programs in a terminal.

### Steps
1. **Clone the repository** (or download the `.cpp` file):
   ```sh
   git clone https://github.com/yourusername/Credit-Card-Validator.git
   cd Credit-Card-Validator
   ```
2. **Compile the program**:
   ```sh
   g++ credit_card_validator.cpp -o validator
   ```
3. **Run the program**:
   ```sh
   ./validator
   ```
4. **Enter a credit card number** to check if it is valid.
5. **Type 'exit'** to quit the program.

## Code Explanation
The program consists of:
1. **Input Handling**: It reads the credit card number from the user and ensures only numerical values are entered.
2. **Luhn Algorithm Implementation**:
   - Every second digit (from right) is doubled.
   - If doubling results in a two-digit number, its digits are summed.
   - The sum is then added to the sum of digits that were not doubled.
   - If the total is a multiple of 10, the number is valid.
3. **Validation Output**: Displays "Valid!" if the card number is correct, otherwise "Invalid!".

## Example Output
```
This program uses the Luhn Algorithm to validate a CC number.
You can enter 'exit' anytime to quit.

Please enter a CC number to validate: 4532015112830366
Valid!

Please enter a CC number to validate: 1234567890123456
Invalid!

Please enter a CC number to validate: exit
```
