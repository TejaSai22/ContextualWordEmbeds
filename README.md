# ContextualWordEmbeds
Just exploring and playing around with few models.

BERT: Some intro and code demonstration!

You can extract the embedding for a specific word/ in the sentence (e.g., the word "bank") and show how BERT's contextual embeddings vary depending on the sentence. This is useful for showcasing polysemy (words with multiple meanings).

The output shape indicates that there is 1 sentence (batch size) with 9 tokens (including the tokens for words like "I," "went," etc.), and each word is represented as a 768-dimensional vector.
This gives a vector representation of the word "bank" in the context of this sentence, where the vector has 768 dimensions. You can repeat this with a different context to see how the vector changes.
2. BERT uses the special [CLS] token to represent the whole sentence. You can extract this embedding to demonstrate how BERT provides sentence-level embeddings.
This is the vector representation of the entire sentence, generated from the [CLS] token, which can be used in tasks like sentence classification.


3. BERT consists of multiple layers, with each producing different levels of contextual representations. You can extract embeddings from each layer and show how the representations change.

The embedding for "bank" evolves as it moves through the layers of BERT. The first layer typically represents more general features, while the last layer encodes more contextual and task-specific information.

4. To demonstrate how BERT captures relationships between words, you can compute the similarity between two-word embeddings in the same sentence.
 
have a high similarity, indicating that they are semantically related in this context (both referring to financial terms).

Summary:
These outputs are meaningful because they demonstrate key aspects of BERT's functionality, such as:

The dimensionality of embeddings.
Contextual understanding of words.
Sentence-level embeddings using the [CLS] token.
Comparison of word similarity.
Layer-wise changes in embeddings.
