# Generating Multiple-Choice Questions from Text

This project demonstrates the process of generating Multiple-Choice Questions (MCQs) from a given text input. The notebook leverages advanced NLP models and preprocessing techniques to automate the creation of MCQs, complete with plausible options for each question.

---

## Features
- **Automated Question Generation**: Converts input text into well-formed questions.
- **Multiple-Choice Options**: Generates meaningful distractors to accompany correct answers.
- **Comprehensive Preprocessing**: Includes tokenization, stopword removal, part-of-speech tagging, and candidate selection for accurate question generation.
- **Customizable Workflow**: Adaptable for various use cases and domains.

---

## Models Used

### **T5 Model (Text-To-Text Transfer Transformer)**
- Utilized for conditional text generation.
- Fine-tuned to generate questions from context.

### **Sense2Vec Model**
- An advanced version of Word2Vec.
- Generates sense-aware word vectors to produce plausible distractors.

---

## Methodology

### **Preprocessing Steps**
1. **Text Tokenization**:
   - Splits input text into sentences and words for granular processing.
2. **Stopword Removal**:
   - Filters out irrelevant words to focus on significant content.
3. **Part-of-Speech Tagging**:
   - Identifies nouns and proper nouns essential for generating meaningful questions and options.
4. **Candidate Selection**:
   - Uses the MultipartiteRank algorithm to extract key phrases for question generation.

### **Question and Option Generation**
- **T5 Model**: Generates questions based on selected key phrases.
- **Sense2Vec**: Creates distractors for each question to enhance MCQ quality.

---

## Example Usage

The notebook includes a `PythonPredictor` class that:
- Processes input text.
- Generates MCQs with options.
- Returns questions and options as output.

Example workflow:
1. Instantiate the `PythonPredictor` class.
2. Provide input text to the predictor.
3. Retrieve and review the generated MCQs.

---

## Note
- This project is intended for educational and demonstration purposes.
- Users are encouraged to customize and adapt the code for specific requirements and use cases.


## Installation

Follow these steps to get the project up and running:

1. Clone the repository:

   git clone https://github.com/vrahul2108/MCQ_Generator.git

2. Navigate into the project directory:

   cd Quizz_Generator

3. Create and activate a virtual environment:

    python -m venv .venv
    .\.venv\Scripts\Activate  

4. Install required dependencies:

   pip install -r requirements.txt

5. Download the SpaCy model:

   python -m spacy download en_core_web_sm

6. Run the application:

   python app.py
