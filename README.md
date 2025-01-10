# Sentence Parser and Noun Phrase Extractor  

## Description  
This project implements a natural language parser that determines the structure of sentences and extracts noun phrases using context-free grammar. The parser is built using Python's Natural Language Toolkit (NLTK). Parsing sentence structures helps computers better understand sentences and extract useful information, such as identifying subjects or important noun phrases.  

## Key Features  
- **Sentence Parsing**: Utilizes context-free grammar rules to parse sentences and determine their syntactic structure.  
- **Noun Phrase Extraction**: Identifies and extracts noun phrase chunks, which are the smallest noun phrases without nested noun phrases within them.  
- **NLTK Integration**: Leverages the NLTK library for tokenization, preprocessing, and tree-based grammar manipulation.  

## What I Implemented  
I worked on the following components of the project:  

### Preprocessing Function (`preprocess`)  
- Tokenized sentences using NLTK's `word_tokenize` function.  
- Converted all tokens to lowercase and filtered out tokens without alphabetic characters.  
- Ensured that the processed tokens were ready for parsing.  

### Grammar Rules (`NONTERMINALS`)  
- Designed and implemented context-free grammar rules to handle complex sentence structures and generate valid parses for all test sentences in the dataset.  
- Created rules to support various types of noun phrases and syntactic combinations while avoiding over-generation or under-generation of sentences.  

### Noun Phrase Chunking Function (`np_chunk`)  
- Implemented logic to extract noun phrase chunks from the syntax tree of a sentence.  
- Ensured that only non-nested noun phrases were identified and returned as `nltk.tree` objects.  
