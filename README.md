# Word-Embedding-Techniques-Word2Vec-BERT-and-Doc2Vec-for-Text-Vectorization-
# Summary: Word Embedding Techniques (Word2Vec, BERT, and Doc2Vec) for Text Vectorization

In this notebook, we explore and apply three popular methods for generating vector representations (embeddings) of text data: **Word2Vec**, **BERT**, and **Doc2Vec**. These methods are essential for converting text into numerical vectors that can be used in various NLP tasks such as text classification, clustering, and more.

1. **Word2Vec**:
   - **Description**: Word2Vec is a neural network-based model that learns vector representations of words from large text corpora. It captures the semantic relationships between words by learning from context.
   - **Advantages**:
     - Flexible and customizable for specific tasks.
     - Efficient for small to medium-sized datasets.
   - **Disadvantages**:
     - Slower when working with large datasets.
     - May experience performance issues when adding too many columns to the DataFrame.
   
   **Note**: In this notebook, **Word2Vec** is used to generate word embeddings by training the model on the text data and then averaging word vectors to generate sentence embeddings.

2. **BERT**:
   - **Description**: BERT (Bidirectional Encoder Representations from Transformers) uses a transformer-based model to generate **contextualized embeddings**. Unlike traditional embeddings, BERT considers the surrounding context of words to generate more accurate representations.
   - **Advantages**:
     - Highly accurate and context-aware embeddings.
     - Suitable for tasks requiring deep understanding of language context.
   - **Disadvantages**:
     - Computationally expensive and slower than other methods.
     - Requires significant memory and resources, making it less efficient for very large datasets.
   
   **Note**: **BERT** is applied here to generate more context-aware sentence embeddings. These embeddings capture the meaning of words depending on their surrounding context.

3. **Doc2Vec**:
   - **Description**: Doc2Vec extends the Word2Vec approach by generating embeddings not just for words, but for entire documents or sentences. This method captures the overall meaning of larger text chunks, making it useful for document-level tasks.
   - **Advantages**:
     - Great for handling larger documents and capturing the meaning of whole sentences or paragraphs.
     - Works well for tasks requiring the understanding of full text.
   - **Disadvantages**:
     - Training can be computationally intensive.
     - May not offer as much control over individual words compared to **Word2Vec**.
   
   **Note**: **Doc2Vec** is used here to generate embeddings that represent entire documents or sentences, helping capture the semantic meaning beyond individual words.

### **How to Use**:
- **Word2Vec** is used for learning word embeddings and generating sentence representations by averaging the word vectors.
- **BERT** is used to create contextualized embeddings, where the meaning of a word is influenced by the surrounding context.
- **Doc2Vec** is applied to generate document-level embeddings, offering a higher-level representation of text.

In this notebook, we demonstrate how to use each of these methods to generate embeddings for text data and save the results as a CSV file for further analysis.
