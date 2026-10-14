📚 WikiQuiz — Wikipedia-Based Quiz Generator

WikiQuiz is a Python-based educational quiz application that uses structured Wikimedia Wikipedia data to help users learn about different topics through automatically generated multiple-choice questions.

🎯 Project Objective

The objective of WikiQuiz is to make learning more interactive by converting information from Wikipedia articles into short quizzes. Users can enter a topic, find relevant content in the dataset, answer questions, and check their score.

✨ Features

- Topic Search: Search the provided Wikimedia dataset using a topic or keyword.
- Article Retrieval: Retrieve matching content from the dataset.
- Automatic Question Generation: Generate fill-in-the-blank questions from article text.
- Multiple-Choice Questions: Provide four answer options for generated questions.
- Answer Validation: Check submitted answers against the correct answers.
- Score Calculation: Calculate and display the final quiz score.
- Gradio Interface: Provide a simple browser-based interface for generating a quiz.

🛠️ Technologies Used

- Python
- Pandas — data loading and processing
- PyArrow — Parquet file support
- Regular Expressions ("re") — text processing
- Random — question and option selection
- Gradio — user interface

📂 Dataset

WikiQuiz is designed to use the Wikimedia Structured Wikipedia Dataset provided for this project.

The application expects a compatible Parquet dataset file. The dataset should be obtained from the source authorized by the project organizers.

Note: The dataset is not included in this repository. Follow the dataset's access and usage requirements before downloading or sharing it.

⚙️ Setup and Installation

1. Clone the repository

git clone https://github.com/nishchitham-00/wikiQuiz.git
cd wikiQuiz

2. Install the dependencies

pip install pandas pyarrow gradio

3. Prepare the dataset

Obtain the authorized Wikimedia dataset and place the Parquet file in the location configured in the application.

Update the dataset path in the Python code to match your file location.

4. Run the application

After the application has been cleaned up for normal Python execution, run:

python app.py

The Gradio interface will provide a local URL that you can open in your browser.

🚀 How It Works

1. The application loads the Wikimedia dataset.
2. It identifies available text fields.
3. The user enters a topic.
4. The application searches for matching content.
5. It extracts sentences and generates fill-in-the-blank questions.
6. It creates multiple-choice options.
7. The quiz checks answers and calculates the score.

📌 Current Project Scope

This is a prototype intended for educational use. Question quality depends on the available article text and the question-generation method.

Potential future improvements include:

- True/False questions
- Difficulty levels
- Improved distractor generation
- Interactive answer submission and feedback
- Timer and quiz history
- Better handling of missing or short article text

👥 Project Information

Project Name: WikiQuiz
Category: Educational Technology / Quiz Application
Language: Python
Repository: "GitHub — wikiQuiz" (https://github.com/nishchitham-00/wikiQuiz)

📄 Disclaimer

WikiQuiz is an educational project. Wikipedia content and dataset usage remain subject to the applicable licensing terms and project guidelines.
