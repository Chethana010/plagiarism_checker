### Plagiarism Checker

#### Overview
Plagiarism Checker is a Python application that enables users to detect similarity between text files in a specific directory using TF-IDF vectorization and cosine similarity metrics. It visually represents similarity scores between pairs of documents using a heatmap, providing an intuitive means of identifying potential plagiarism.

#### Prerequisites
- Python 3.x
- `scikit-learn`
- `matplotlib`
- `seaborn`

You can install the necessary packages using pip:
```bash
pip install scikit-learn matplotlib seaborn
```

#### Usage
1. Clone the repository.
   ```bash
   git clone [Your Repository Link]
   cd [Your Repository Directory]
   ```
2. Add the text files you wish to check for plagiarism to the `files` directory.
   
3. Run the Plagiarism Checker.
   ```bash
   python plagiarism_checker.py
   ```
4. Review the similarity results in the console and the generated heatmap.

#### How It Works
- **File Retrieval**: All text files from the specified directory are listed.
  
- **Preprocessing**: The contents of the text files are read and preprocessed, converting them to lowercase to ensure consistency in comparison.
  
- **Similarity Check**:
  - TF-IDF Vectorization: Converts text data into numerical format, considering both the frequency of words in a document and the uniqueness of words across documents.
  - Cosine Similarity: Determines the cosine of the angle between two vectors, representing the similarity between two documents.
  
- **Result Presentation**:
  - Console: Similarity scores between each pair of files are printed.
  - Heatmap: A visual representation of the similarity matrix, allowing easy identification of highly similar documents.

#### Files in the Repository
- `plagiarism_checker.py`: Main Python script to check for plagiarism.
- `/files`: Directory to place the text files you want to check for plagiarism.

#### Example
An example is provided within the repository with sample text files to demonstrate the functionality of the Plagiarism Checker.

#### Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

#### License
[MIT License](https://choosealicense.com/licenses/mit/)
