# Quiz MCQ Generator

This is a Python-based project that generates multiple-choice questions (MCQs) based on given text content. The app utilizes NLP (Natural Language Processing) with SpaCy to process the text and extract key information for generating questions.

## Features
- Generate MCQs from input text.
- Display the questions along with multiple choices.
- Built with Python and Flask framework.

## Tech Stack
- **Python**: Programming language used for backend logic.
- **Flask**: A micro web framework to serve the application.
- **SpaCy**: NLP library used to process the text and generate questions.
- **HTML/CSS**: Used for the front-end user interface.

## Installation

Follow these steps to get the project up and running:

1. Clone the repository:

   git clone https://github.com/vrahul2108/MCQ_Generator.git

2. Navigate into the project directory:

   cd QuizMCQ_Generator

3. Create and activate a virtual environment:

    python -m venv .venv
    .\.venv\Scripts\Activate  

4. Install required dependencies:

   pip install -r requirements.txt

5. Download the SpaCy model:

   python -m spacy download en_core_web_sm

6. Run the application:

   python app.py
