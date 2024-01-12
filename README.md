# Evaluation of RAG Models with and without Cross Encoder Reranker

## Project Overview
This project evaluates the performance of the RAG (Retrieval-Augmented Generation) model enhanced with a Cross Encoder Reranker, using the Zephyr 7B Alpha 5 bit Quantised model (BAAI/bge-small-en-v1.5). The model was tested with a comprehensive document titled "Brains in Space: Effects of Spaceflight on the Human Brain and Behavior" spanning 311 pages.

![Results](Advanced-RAG-with-Cross-Encoder-Reranker.png) 

<img src="Advanced-RAG-with-Cross-Encoder-Reranker.png" alt="Alt text for the image">
## Test Methodology
Three questions were posed to assess the model's understanding and contextual accuracy:

A query from the top of the document.
A question from the middle.
An inquiry from the end of the document.

Two configurations were tested:
1. Advanced RAG with Cross Encoder Reranker
2. RAG without Cross Encoder Reranker
   
## Results
### Advanced RAG with Cross Encoder Reranker
Performance: High accuracy with only one material mistake.
Context and Reference Handling: Maintained correct context and accuracy throughout the document.
Response Time: Slower, averaging around 30-45 seconds per response.

Example Responses
Question 1 (DTCost): Detailed and contextually accurate explanation.
Question 2 (Polysomnography): Comprehensive and medically accurate description.
Question 3 (Artificial Gravity and SANS): Thorough analysis with relevant spaceflight information.

### RAG without Cross Encoder Reranker
Performance: Faster response times but compromised accuracy.
Context and Reference Handling: Failed to maintain the correct context or understand the intent for the second and third questions.
Response Time: Significantly faster, averaging around 17-32 seconds per response.

Example Responses
Question 1 (DTCost): Accurate but less detailed.
Question 2 (Polysomnography): More generic, less detailed than the enhanced model.
Question 3 (Artificial Gravity and SANS): Lacked direct mention of SANS, indicating a contextual misunderstanding.

## Conclusion
The RAG model with Cross Encoder Reranker demonstrates superior performance in terms of accuracy and contextual understanding, albeit at the cost of longer response times. In contrast, the standard RAG model, while faster, shows limitations in understanding and contextual accuracy, particularly for complex and specific queries.

This evaluation highlights the trade-off between speed and depth of understanding in AI models, underscoring the importance of choosing the right configuration based on the application's requirements.
