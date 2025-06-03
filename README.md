🏏 AI Commentary for Cricket – MSc Project
This project explores the application of Natural Language Processing (NLP) to generate real-time, human-like cricket commentary based on structured ball-by-ball data. Developed as part of an MSc research project, the system leverages deep learning and sequence modeling to simulate professional sports commentary in response to live match inputs.

📊 Dataset Overview
Total records: 712,050 rows (ball-by-ball cricket match data)

Columns used: Over number, batsman, bowler, runs, wicket, extras, commentary (text)

After preprocessing:

Unique batsmen: 682

Unique bowlers: 493

Total unique commentary phrases: 28,000+

📁 Notebooks
🔍 EDA.ipynb
Conducted in-depth analysis of player performance, over patterns, and commentary structure.

Visualized key features such as run distribution, bowler variety, and over progression.

Encoded text and cleaned commentary data for model compatibility.

Generated sample word clouds and word frequency distributions to analyze common commentary terms.

🤖 MODEL_BUILDING.ipynb
Used token-based text generation to simulate realistic commentary from numeric match events.

Tokenization: Custom tokenizer with 3,091 unique tokens (words).

Input sequence length: 25

Model architecture:

Embedding Layer → LSTM Layer → Dense Output Layer

Optimizer: Adam | Loss Function: Categorical Crossentropy

📈 Model Performance
Training Accuracy: 90.71%

Validation Accuracy: 87.84%

Training Loss: 0.3845

Validation Loss: 0.4767

Epochs trained: 100

Best results were achieved after early stopping at epoch 77 due to overfitting signs beyond that point.

Sample Output:

Input: "Over 18.5 | Bumrah to Dhoni | Yorker | Dot Ball"

Generated Commentary: "Another perfect yorker by Bumrah! Dhoni fails to score. Pressure mounts on Chennai!"

⚙️ Tools & Technologies
Language: Python

Libraries: Pandas, NumPy, Matplotlib, Seaborn, TensorFlow (Keras), NLTK

Modeling: LSTM-based sequence generation with text tokenization

Evaluation: Accuracy, loss graphs, and output comparison to real commentary

💡 Project Outcome
This project demonstrates how NLP and deep learning can be applied to automate real-time cricket commentary generation with high accuracy and context alignment. The system can be extended to multilingual support, live match streaming integration, and deployment as a web or mobile application.
