# NLP-Rubrics-----News-Summarizer

Introduction:
The vast amount of textual information available on the internet and news portals makes it difficult for readers to quickly grasp the essential points of an article. Text summarization, an important application of Natural Language Processing (NLP), helps condense lengthy articles into concise summaries.
This project implements a simple extractive summarization model using Python. It allows the user to input a passage (up to 250 words), and the system generates a shorter summary highlighting the most significant sentences.

Objectives:
•	To design an NLP-based text summarization tool.
•	To implement sentence tokenization and word frequency–based scoring.
•	To provide concise summaries that retain the meaning of the original text.

Methodology:
1.	Preprocessing:
o	Text is tokenized into sentences.
o	Words are extracted and converted to lowercase.
o	Stopwords are removed.
2.	Word Frequency Calculation:
o	Each non-stopword is counted to build a frequency dictionary.
3.	Sentence Scoring:
o	Sentences are scored based on the frequency of words they contain.
o	Higher-scoring sentences are considered more important.
4.	Summary Generation:
o	Sentences are ranked by score.
o	The top N sentences are selected to form the summary (maintaining original order).

Tools and Technologies:
•	Language: Python
•	Libraries: nltk, re, collections
•	Environment: Jupyter Notebook



Sample Output:
Input: A news article passage (about a sports champion).
Output: A condensed 3-sentence summary highlighting key achievements.

Results:
•	The summarizer was able to produce coherent summaries.
•	The output successfully reduced long paragraphs into short, readable summaries.
•	Works effectively for short news articles or paragraphs.

Limitations:
•	The model is extractive, not abstractive – it only picks existing sentences instead of generating new ones.
•	Sometimes important context is lost if it falls outside the top-ranked sentences.
•	When AI-generated or synthetic input is applied, the results may be incorrect or insufficient, since the algorithm depends heavily on word frequency and sentence scoring.
•	No semantic understanding (e.g., meaning, tone, or paraphrasing).

Conclusion:
This project demonstrates how basic NLP techniques can be applied to generate summaries. While the approach is simple and efficient, further improvements can be made by integrating more advanced models such as Transformer-based architectures (BERT, GPT) for better contextual understanding and abstractive summarization.
