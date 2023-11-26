# Graduation-project-Swapify


## Overview
Swapify is a hybrid recommendation system designed to connect users based on their preferences for swapping or exchanging products. It combines collaborative filtering and content-based filtering techniques to provide accurate and personalized product recommendations.

## Hybrid Recommendation System
A hybrid recommendation system combines multiple recommendation approaches to overcome the limitations of individual methods. Swapify utilizes both collaborative filtering and content-based filtering to enhance the recommendation process.

### Collaborative Filtering
Collaborative filtering suggests products based on the preferences of users with similar tastes. Swapify identifies potential swap partners by comparing the preferences and swap histories of users. Users who have swapped similar items in the past are considered potential matches.

### Content-Based Filtering
Content-based filtering recommends products based on their features and attributes. Swapify uses natural language processing (NLP) techniques to analyze product descriptions and find similarities between items. This ensures that recommended swaps not only match user preferences but also share similar characteristics.

## Key Features

### 1. User Profiles
- **Location-Based Matching:** Swapify considers the geographical location of users to recommend swaps with nearby users.
- **Swap and Wish Lists:** Users maintain lists of items they are willing to swap and items they are looking for, forming the basis of the recommendation system.

### 2. Matching Algorithm
- **Cosine Similarity:** The matching algorithm calculates the cosine similarity between item descriptions using the SentenceTransformer model. This ensures that recommended items not only align with user preferences but also have similar textual features.

### 3. MongoDB Integration
- **User and Product Data Storage:** Swapify stores user profiles, swap lists, and wish lists in MongoDB, providing a scalable and efficient solution for data management.

## Getting Started

### Dependencies
Ensure you have the required dependencies installed. Use the following command to install them:

```bash
!pip install transformers
!pip install sentence-transformers
!pip install faiss-cpu
!pip install -U sentence-transformers
!pip install pymongo
```

### Running Swapify
1. **MongoDB Connection:** Set up a MongoDB instance and provide the connection details in the `get_user_list` function.
2. **Execute Code:** Run the provided code to fetch user lists, find similarities, and save the results to a JSON file.

## Usage
1. **User Registration:** Users create profiles and populate swap and wish lists.
2. **Run Matching Algorithm:** Execute the matching algorithm to find potential swap partners based on user preferences and product descriptions.
3. **Review Recommendations:** Explore the recommendations stored in the 'matching_items.json' file.

## Conclusion
Swapify offers a comprehensive hybrid recommendation system that combines collaborative and content-based filtering. By considering both user preferences and product characteristics, Swapify provides accurate and diverse recommendations, enhancing the user experience in the swapping community.
