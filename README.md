# Goal
This work presents a comprehensive approach to language identification and language similarity analysis using character-level trigram language models and byte-pair encoding (BPE). Our goal is to accurately classify sentences into their respective languages and explore the similarities between languages based on subword tokenization. 

# Dataset
The dataset we are using comes from wikipedia and is a collection of five different datasets, each corresponding to a different language. The languages included in the dataset are Dutch (’nl’), Afrikaans (’af’), Xhosa (’xh’), English (’en’), and Zulu (’zu’).
There is a separate training ( 2000 rows and 1 column) and validation ( 1000 rows and 1 column) file for each language, where each row is a sentence in that language. The test data is a single dataset (1000 rows and 1 column) which contains all languages such a way that the first two characters on each line indicate the language of the sentence and the rest of the line is the sentence, which the model will take as input. The validation data has been normalized so that the sentences match the form of the test data. For each language, the training data is in its original form, this means that we will normalize the training data to match the form of the validation data (and by implication the test data).

# Result
The language identification task involves training lan- guage models specific to each language and achieving a high accuracy of 90.8% in identifying languages in the test data. The BPE technique allows for the analysis of language similarity by identifying shared subword units between languages. The results demonstrate the effectiveness of the proposed framework in accu- rate language identification and capturing language similarities without relying on external NLP toolkits.



 # The notebook is well documented and commented. Just follow each step and read the comment after each cell.
