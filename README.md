# UniqueTokenExtractor

Unique Token Extractor is an open-source Python application designed to compare the vocabularies of two language models (LLMs) and extract the unique tokens present in each model. This tool provides insights into the differences between the vocabularies of the models, which can be useful for understanding their capabilities and potential for merging.

Features
Compare vocabulary sizes of two language models
Calculate the overlap between the vocabularies
Extract and display the unique tokens present in each model
Installation
Clone the repository:

Copy code
git clone https://github.com/RichardAragon/unique-token-extractor.git
Install the required dependencies:

Copy code
pip install -r requirements.txt
Usage
Run the unique_token_extractor.py script and follow the prompts to enter the names of the two models you want to compare:


Copy code
python unique_token_extractor.py
The script will output the following information:

Vocabulary sizes of both models
Number of overlapping tokens between the vocabularies
Number of unique tokens in each model
Lists of unique tokens for each model
Example Output

Copy code
Enter the name of the first model: bert-base-uncased
Enter the name of the second model: roberta-base

Comparing vocabulary sizes:
Vocabulary size - bert-base-uncased: 30522, roberta-base: 50265
Vocabulary overlap: 28996
Unique tokens in bert-base-uncased: 1526
Unique tokens in roberta-base: 21269

Unique tokens in bert-base-uncased:
['-', '[', ']', '§', '€', '₹', '←', '↑', '→', '↓', '⇄', '⇌', '⇒', '≈', '≥', '─', '│', '■', '▶', '◄', ...]

Unique tokens in roberta-base:
['Ġ-', 'Ġ[', 'Ġ]', 'Ġ§', 'Ġ€', 'Ġ₹', 'Ġ←', 'Ġ↑', 'Ġ→', 'Ġ↓', 'Ġ⇄', 'Ġ⇌', 'Ġ⇒', 'Ġ≈', 'Ġ≥', 'Ġ─', 'Ġ│', 'Ġ■', 'Ġ▶', 'Ġ◄', ...]
Requirements
Python 3.7 or higher
Transformers
Contributing
Contributions are welcome! If you find any issues or have suggestions for improvements, please open an issue or submit a pull request.

License
This project is licensed under the MIT License.

Acknowledgements
This project utilizes the Transformers library by Hugging Face.
We would like to thank the open-source community for their valuable contributions and inspiration.
