# CONFER: A Dataset for Presupposition and CONditional InFERence Evaluation
[![License: CC BY 4.0](https://img.shields.io/badge/License-CC%20BY%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by/4.0/)


CONFER is a curated dataset of 18,000 sentence pairs in natural language inference (NLI) format, developed to investigate how language models handle presuppositions in specific types of conditional sentences. For more on the NLI task, see the [Stanford NLI project](https://nlp.stanford.edu/projects/snli/).

The dataset was introduced in our paper "Let’s CONFER: A Dataset for Evaluating Natural Language Inference Models on CONditional InFERence and Presupposition", where we probe both symbolic models and large language models on their ability to make inferences based on different conditional structures.

**Link to Paper**: TBA






## Dataset Overview

The CONFER dataset contains sentence pairs designed to evaluate model understanding of the relationship between a conditional sentence (premise) and its potential presupposition (hypothesis), where the presupposition trigger appears in the antecedent of the conditional. Each example includes a premise-hypothesis pair and a gold label (`E`, `C`, or `N`) representing their inferential relationship under the assumption that the premise is true.

| Type | Trigger     | Premise                                                                 | Hypothesis                      | Label |
|------|-------------|-------------------------------------------------------------------------|----------------------------------|--------|
| 1    | again       | *Sam believes that if Nadia adopted a cat, she will never adopt a cat again.* | Nadia adopted a cat.            | N      |
| 2    | possessive  | *If Marley has an outgoing friend, she travels with her friend.*        | Marley has a friend.            | N      |
| 3    | again       | *If Ryan ever watched a movie, he didn't watch Star Wars again.*        | Ryan watched Star Wars again.   | C      |
| 4    | possessive  | *If George has a dog, I wonder how loud George's dog barks.*            | George has a dog.               | N      |
| 5    | possessive  | *It's not the case that if Scarlett finishes her work early, her brother will take her out for dinner.* | Scarlett has a brother. | E      |

**Label Key:**  
- `E` = Entailment  
- `C` = Contradiction  
- `N` = Neutral





## Usage

The scripts and prompt templates for both data generation and model evaluation are included in this repository. You are welcome to experiment with or adapt them for your own research. For a detailed description of the generation and evaluation procedures, please refer to the accompanying paper.

**Download the Dataset:**  
The dataset is also available on the [Hugging Face Datasets Hub](https://huggingface.co/ConditionalNLI/CONFER).




## Citation




## License

This repository is licensed under the [Creative Commons Attribution 4.0 International License (CC BY 4.0)](https://creativecommons.org/licenses/by/4.0/).

You are free to share, use, and adapt the dataset, prompts, and documentation for any purpose, provided that proper credit is given to the authors.




