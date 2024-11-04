# AI Knowledge Representation with Python Logic Code

This project demonstrates *AI Knowledge Representation* using propositional logic and symbolic reasoning to solve various logic-based puzzles. Each Python file showcases different aspects of logical representation, inference, and model checking.

## Table of Contents
- [Project Overview](#project-overview)
- [File Descriptions](#file-descriptions)
- [Getting Started](#getting-started)
- [Usage](#usage)
- [Dependencies](#dependencies)
- [License](#license)

## Project Overview
Knowledge Representation (KR) is essential in AI for encoding information in a way that allows machines to reason and make logical inferences. This project uses *symbolic logic* to represent knowledge in the form of propositions, and employs logical operators (AND, OR, NOT, Implication) to enforce rules and derive conclusions.

The core logic is implemented in logic.py, while other files build knowledge bases and query them to solve specific problems or make decisions. This approach is useful in AI applications such as game solving, rule-based systems, and decision-making under constraints.

## File Descriptions

### logic.py - Core Logic Engine
The logic.py file provides classes and methods to create logical sentences, evaluate models, and check entailments:
- *Symbol*: Represents atomic propositions, such as game elements or events.
- *Logical Connectives*: Classes for And, Or, Not, Implication, and Biconditional, which combine propositions to form complex logical sentences.
- *model_check*: A function that verifies if a set of knowledge statements entails a particular query, using truth assignments.

### clue.py - Clue Game Logic Representation
This file models a simplified Clue game:
- *Symbols* represent characters (e.g., ColMustard), rooms (e.g., ballroom), and weapons (e.g., knife).
- *Knowledge Base*: Rules of the game, such as each category having one item, are encoded with logical constraints.
- *Inference*: Uses model_check to determine possible characters, rooms, and weapons based on given clues.

### harry.py - Simple Implications and Constraints
This script represents basic implications and exclusivity:
- *Symbols* represent events or people (e.g., rain, hagrid).
- *Logical Rules*: Constructs simple conditional statements (e.g., if not raining, Hagrid is present).
- *Query*: Uses model_check to infer whether it’s raining.

### mastermind.py - Mastermind Puzzle Constraints
Models a Mastermind-like puzzle:
- *Symbols* represent color-position assignments (e.g., red0, blue1).
- *Knowledge Base*: Ensures each color occupies one position and prevents multiple colors in the same position.
- *Inference*: Derives possible color arrangements using initial clues and model_check.

### puzzle.py - Hogwarts House Assignment
Represents Hogwarts house assignments with constraints:
- *Symbols* represent each person-house pairing (e.g., GilderoyGryffindor).
- *Logical Constraints*: Each person is assigned one house, and each house has one person.
- *Inference*: Uses model_check to confirm valid assignments based on clues provided.

## Getting Started

### Prerequisites
- *Python 3.x*
- Required libraries specified in [Dependencies](#dependencies).

### Installation
1. Clone the repository:
   bash
   git clone https://github.com/your-username/ai-knowledge-representation.git
   
2. Navigate to the directory:
   bash
   cd ai-knowledge-representation
   
3. Install dependencies:
   bash
   pip install -r requirements.txt
   

## Usage
Run each script independently to test logical inference in various scenarios:
bash
python clue.py
python harry.py
python mastermind.py
python puzzle.py


Each script will output results based on the logical constraints encoded within its knowledge base.

## Dependencies
- *termcolor*: For color-coded terminal output.
- *Python Standard Library*: Only uses standard library modules other than termcolor.

Install with:
bash
pip install termcolor


## License
This project is licensed under the MIT License. See LICENSE for more details.

