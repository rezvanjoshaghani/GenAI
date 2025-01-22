# HomeMatch Application

## Overview

The HomeMatch application is designed to generate real estate listings and match them with buyer preferences using a Large Language Model (LLM) and a vector database for semantic search. This project implements two different solutions to address the requirements effectively.

### Solutions Implemented

#### Solution 1: Direct LLM Generation & Matching

1. Generating Real Estate Listings

- Utilized OpenAI's GPT model to generate at least 10 diverse and realistic real estate listings.

- Listings include details such as neighborhood, price, bedrooms, bathrooms, size, and descriptions.

- Listings are saved in a JSON file to reduce API call costs.

2. Storing Listings in a Vector Database

- Listings are processed into embeddings using OpenAI Embeddings.

- ChromaDB is used as the vector database to store these embeddings.

3. Semantic Search Based on Buyer Preferences

- Buyer preferences are collected through structured questions.

- Preferences are parsed into a summary and converted into embeddings.

- A similarity search is performed on the vector database to find the best-matching listings.

4. Personalized Listing Descriptions

- The retrieved listings are reprocessed using the LLM to personalize descriptions based on buyer preferences.

- Ensures factual integrity while enhancing the appeal of listings.

#### Solution 2: Conversational Recommendation System

1. Interactive Buyer Preference Collection

- Implemented a conversational AI interface to interactively gather buyer preferences.

- Memory management using LangChain's ConversationSummaryMemory and ConversationBufferMemory.

2. Enhanced Recommendation System

- Buyer persona is created based on structured questions and stored preferences.

- AI generates a rating for each listing based on alignment with buyer preferences.

- Final recommendation is based on the highest-rated listings.

## How to Run the Application

### Prerequisites

- Python 3.8+

- pip install -r requirements.txt

- OpenAI API Key

- ChromaDB installed (pip install chromadb)

### Project Files

- HomeMatch.ipynb - Jupyter Notebook containing all project components including listing generation, vector database storage, and recommendation system.

- listings.json - Pre-generated listings to optimize API usage.

- requirements.txt - List of necessary dependencies.

## Features Implemented

✅ Real Estate Listing Generation
✅ Vector Database for Semantic Search
✅ AI-Powered Matching and Recommendations
✅ Personalized Listing Descriptions
✅ Interactive Buyer Preference Collection
✅ Rating and Recommendation System

## Conclusion

This project showcases two solutions for matching buyers with real estate listings: one leveraging direct LLM-based search and the other using a conversational recommendation system. The combination of semantic search and personalized listing enhancement ensures an optimal user experience.

