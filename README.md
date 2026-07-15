# **Byte Pair Encoding (BPE) Implementation using Python**

## 1. Overview

Byte Pair Encoding (BPE) is a data compression and tokenization algorithm widely used in Natural Language Processing (NLP). It converts words into smaller subword units by repeatedly merging the most frequently occurring pair of characters. This project demonstrates the complete implementation of the BPE algorithm in Python. It reads a corpus from a text file, builds a vocabulary, learns merge rules, generates subword tokens, and tests the encoding and decoding process.

---

# 2. Objective

* To understand the working of the Byte Pair Encoding (BPE) algorithm.
* To implement BPE tokenization using Python.
* To build a vocabulary from a text corpus.
* To identify and merge the most frequent character pairs.
* To encode and decode words using the learned merge rules.
* To demonstrate subword tokenization used in modern NLP models such as GPT and BERT.

---

# 3. Applications

* Natural Language Processing (NLP)
* Large Language Models (LLMs)
* Machine Translation
* Text Compression
* Speech Recognition
* Chatbots and Virtual Assistants
* Search Engines
* Text Classification
* Sentiment Analysis
* Automatic Text Generation

---

# 4. Features

* Reads input words from a **corpus.txt** file.
* Converts words into character-level tokens.
* Builds an initial vocabulary with word frequencies.
* Counts the frequency of adjacent symbol pairs.
* Learns merge rules based on the most frequent pairs.
* Creates a final subword vocabulary.
* Encodes new words using learned merge rules.
* Decodes encoded tokens back to the original words.
* Displays intermediate merge steps and final vocabulary.

---

# 5. Project Structure

```text
Byte-Pair-Encoding/
│
├── corpus.txt              # Input dataset
├── bpe.py                  # Main Python program
├── README.md               # Project documentation
└── Output.txt              # Sample output (optional)
```

---

# 6. Workflow

```
Start
   │
   ▼
Read corpus.txt
   │
   ▼
Convert words into character tokens
   │
   ▼
Build Initial Vocabulary
   │
   ▼
Count Adjacent Character Pairs
   │
   ▼
Find Most Frequent Pair
   │
   ▼
Merge the Pair
   │
   ▼
Repeat Until Required Merges
   │
   ▼
Generate Final Vocabulary
   │
   ▼
Encode New Words
   │
   ▼
Decode Tokens
   │
   ▼
Display Results
   │
   ▼
End
```

---

# 7. Algorithm

**Step 1:** Read all words from the **corpus.txt** file.

**Step 2:** Convert each word into individual characters and append the end-of-word symbol (`</w>`).

**Step 3:** Build the initial vocabulary with word frequencies.

**Step 4:** Count the frequency of every adjacent character pair.

**Step 5:** Select the pair with the highest frequency.

**Step 6:** Merge the selected pair into a single token.

**Step 7:** Repeat the merge process for a fixed number of iterations.

**Step 8:** Construct the final subword vocabulary.

**Step 9:** Encode new words using the learned merge rules.

**Step 10:** Decode the encoded tokens back into the original words.

---

# 8. Technologies Used

| Technology             | Purpose                         |
| ---------------------- | ------------------------------- |
| Python 3.x             | Programming Language            |
| NumPy                  | Frequency calculations          |
| Collections (Counter)  | Counting words and symbol pairs |
| Jupyter Notebook       | Program development and testing |
| Text File (corpus.txt) | Input dataset                   |


<img width="593" height="620" alt="Screenshot 2026-07-15 111837" src="https://github.com/user-attachments/assets/5f607375-637f-443b-9f48-b2fddc38ad31" />
<img width="277" height="366" alt="Screenshot 2026-07-15 112320" src="https://github.com/user-attachments/assets/2f84574c-b423-40d8-8fa6-4ec6dfe7628e" />
<img width="445" height="620" alt="Screenshot 2026-07-15 111916" src="https://github.com/user-attachments/assets/0f05b885-c049-44b3-a52d-4cce491f293d" />

---

# 9. Result

The project successfully implements the Byte Pair Encoding algorithm. It reads words from the input corpus, learns the most frequent character pair merges, constructs a compact subword vocabulary, and accurately encodes and decodes words using the learned merge rules. The output demonstrates how BPE reduces vocabulary size while preserving the ability to reconstruct the original words.

---

# 10. Conclusion

This project provides a practical implementation of the Byte Pair Encoding (BPE) algorithm using Python. It demonstrates how frequent character pairs are merged to create meaningful subword units, improving vocabulary efficiency and handling unknown words effectively. The implementation reflects the tokenization approach used in many modern NLP and Large Language Models, making it a useful educational project for understanding text preprocessing and subword tokenization.
