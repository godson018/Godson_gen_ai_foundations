# Godson_gen_ai_foundations
# Answers

## Question 1: The Vector Conflict

The dot product similarity score may show a non-zero or even relatively high similarity between 
Sentence 1 and Sentence 2 despite the word "light" being used in different contexts. 
This occurs because CountVectorizer uses a bag-of-words representation that only counts word occurrences and ignores meaning. 
Since both sentences contain the word "light" and possibly other overlapping terms, the vectors appear mathematically related. 
Therefore, the model creates a false similarity because it cannot distinguish between different meanings of the same word.

## Question 2: The Context Blindspot

The bag-of-words approach creates a major bottleneck because it removes context, word order, and semantic relationships from text.
Every document is reduced to static word counts, making it impossible to determine the intended meaning of ambiguous words. 
As a result, search engines and chatbots built solely on this method can return inaccurate results when words have multiple meanings. 
The linguistic property that is completely lost is semantic context.

## Question 3: The GenAI Architectural Fix

Modern Large Language Models such as GPT and LLaMA solve this problem using context-aware embeddings and self-attention mechanisms. 
Context-aware embeddings generate different vector representations for the same word based on the surrounding words in a sentence. 
Masked Self-Attention analyzes relationships between words and helps the model understand how each word contributes to the overall meaning. 
Together, these techniques ensure that the word "light" receives different mathematical vectors when referring to low-calorie products,
physical weight, or illumination.
