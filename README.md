# Text Analysis Assignment

## Objective
The aim of this assignment is to create a series of Python functions for basic text analysis. You will work with a provided corpus of text and a file of stop words. Your task is to work with this data in the way described in the tasks below.

## Instructions

### Setup
- Ensure Python is installed in your system.
- Only standard library required. (Please do not use any external libraries like `nltk`, `pandas`, etc.)
- Two files are provided: `corpus.txt` containing the text data and `stop_words.txt` listing common stop words separated by comma.

### Tasks
1. **Read Corpus**
   - Implement a function `read_corpus(filename: str) -> list[str]` that reads text from `corpus.txt` split it into list of words (tokens separated by space) returns it as a list of strings.

2. **Read Stop Words**
   - Implement a function `read_stop_words(filename: str) -> list[str]` that reads stop words (comma separated) from `stop_words.txt` and returns them as a list of strings.

3. **Process**
   - Implement a function `process(corpus: list[str]) -> list[str]` that takes the corpus as a list and converts each word to lowercase.

4. **Remove Stop Words**
   - Implement a function `remove_stop_words(corpus: list[str], stop_words: list[str]) -> list[str]` that removes stop words from the corpus.

5. **Identify K-th Most Frequent Word**
   - Implement a function `find_kth_frequent_word(corpus: list[str], k: int) -> tuple[str, int]` that identifies the K-th most frequent word in the corpus and its count.

6. **Identify Average Length of Word in Corpus**
   - Implement a function `find_average_word_length(corpus: list[str]) -> float` that returns the mean length of the word in the corpus.

### Example Usage
```python
corpus = read_corpus('corpus.txt')
stop_words = read_stop_words('stop_words.txt')
words = process(corpus)
words = remove_stop_words(words, stop_words)
kth_word = find_kth_frequent_word(words, 1)
print(f'Second Most Common Word: {top_words}')
mean_length = find_mean_word_length(words)
print(f'Average word length: {max_length}')
```

## Evaluation Criteria
1. **Correctness**: The implemented functions should correctly perform the tasks as described.
2. **Code Quality**: Your code should be clear, concise, and well-documented.
3. **Efficiency**: Your implementation should efficiently handle the text processing and analysis tasks.
4. **Pythonic Practices**: Use of Pythonic coding style.
