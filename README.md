# neolen-assignment

# Medical details Extraction and Classification

## Objective
The objective of this project is to create structured data of details from a scanned bill of items document, and then classify data as either medical or non-medical.

## Overview
This project uses a combination of OCR (Optical Character Recognition), language models, and a custom classification system to achieve the desired outcome. The key steps involved are:

1. **PDF Extraction**: The text content is extracted from the scanned PDF document using OCR techniques.
2. **Text Preprocessing**: The extracted text is cleaned and formatted to prepare it for further processing.
3. **Embedding Generation**: The cleaned text is converted into embeddings using a language model, which allows for efficient storage and retrieval of the document content.
4. **Vector Store Creation**: The document embeddings are stored in a vector store, which enables efficient querying and retrieval of relevant content.
5. **Prompt Engineering**: A custom prompt template is designed to guide the language model in extracting the desired information from the document.
6. **Item Extraction**: The language model is invoked using the prompt template to extract the item details, including name, quantity, rate, and amount.
7. **Item Classification**: The extracted item details are classified as either medical or non-medical using a custom classification system.

## Technical Approach
The technical approach for this project involves the following key components:

1. **OCR Library**: The `pdf2image` and `pytesseract` libraries are used to extract text from the scanned PDF document.
2. **Language Model**: The `ChatOpenAI` model from the `langchain-openai` library is used for text extraction and embedding generation.
3. **Vector Store**: The `Chroma` vector store from the `langchain-chroma` library is used to store and retrieve the document embeddings.
4. **Prompt Engineering**: A custom prompt template is designed using the `ChatPromptTemplate` from the `langchain-core` library.
5. **Output Schema**: The `Pydantic` library is used to define the output schema for the extracted item details.
6. **Classification System**: A custom classification system is implemented to categorize the extracted items as either medical or non-medical.

## Workflow
The overall workflow of the project is as follows:

1. **PDF Extraction**: The text content is extracted from the scanned PDF document using OCR techniques.
2. **Text Preprocessing**: The extracted text is cleaned and formatted to prepare it for further processing.
3. **Embedding Generation**: The cleaned text is converted into embeddings using the language model.
4. **Vector Store Creation**: The document embeddings are stored in a vector store for efficient retrieval.
5. **Prompt Engineering**: A custom prompt template is designed to guide the language model in extracting the desired information from the document.
6. **Item Extraction**: The language model is invoked using the prompt template to extract the item details, including name, quantity, rate, and amount.
7. **Item Classification**: The extracted item details are classified as either medical or non-medical using a custom classification system.

## Results and Insights
The results of the item extraction and classification process will be presented in the following format:

1. **Extracted Item Details**: A table or list of the extracted item details, including name, quantity, rate, and amount.
2. **Item Classification**: The classification of each item as either medical or non-medical.
3. **Insights and Observations**: Any insights or observations drawn from the extracted data and classification results.

## Future Enhancements
Potential future enhancements for this project include:

## Conclusion
This project demonstrates the application of OCR, language models, and custom classification systems to extract and categorize item details from scanned bill of items documents. The insights and findings from this project can be used to streamline inventory management, optimize medical supply procurement, and enhance overall operational efficiency in the healthcare sector.
