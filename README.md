Named Entity Recognition on News Articles

This project demonstrates a basic **Named Entity Recognition (NER) pipeline using spaCy.  
The goal is to identify entities such as PERSON, ORGANIZATION, LOCATION, and DATE** from news article text.

A small labeled dataset was used to train and evaluate the model for learning and demonstration purposes.

Technologies Used:
- Python  
- spaCy  
- pandas  
- scikit-learn  
- Jupyter Notebook  

Project Structure:

Entity Recognition Project/
│
├── data/
│ ├── labeled_news.json
│ └── new_articles.txt
│
├── outputs/
│ └── annotated_articles.txt
│
├── reports/
│ └── evaluation_metrics.txt
│
├── ner_news_project.ipynb
└── README.md

Approach:
1. Loaded a small labeled news dataset  
2. Converted data into spaCy training format  
3. Trained a custom Named Entity Recognition model  
4. Evaluated the model using precision, recall, and F1-score  
5. Applied the trained model to annotate new news articles  

Evaluation:
The model was evaluated on a small test set using:
- Precision  
- Recall  
- F1-score  

Evaluation results are stored in:
reports/evaluation_metrics.txt

Sample Output
Example annotated sentence:
[ORG]Apple[/ORG] was founded by [PERSON]Steve Jobs[/PERSON] in [GPE]California[/GPE].

How to Run
1. Install dependencies:
pip install spacy pandas scikit-learn
python -m spacy download en_core_web_sm

Then Open Jupyter Notebook and run:
ner_news_project.ipynb

Note:
This project uses a small dataset for demonstration and learning purposes.
Model performance can be improved by increasing dataset size and label diversity.




