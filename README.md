# Topic_Analysis_of_Clothing_Reviews_with_Embeddings
Analyzed clothing reviews on an e-commerce platform to explore different topics and similarities among them

# Clothing Review Topic Analysis: Semantic Search & Theme Discovery with OpenAI Embeddings | Python, t-SNE

Turned thousands of free-text e-commerce reviews into vector embeddings to surface customer themes and find similar reviews by meaning, not keywords. A 2D map of the embeddings shows how feedback groups into topics.

# CONTEXT
Customer feedback is a goldmine, but unstructured text is hard to scale. I used the Women's Clothing E-Commerce Reviews dataset to explore what customers talk about and how to retrieve related feedback quickly.

# MY ROLE
I handled text preparation, embedding generation, dimensionality reduction, visualisation, topic categorisation and similarity search.

# WHAT I DID
• Cleaned the 'Review Text' column by handling missing reviews and generated embeddings with the modeltext-embedding-3-small via the OpenAI API.
• Reduced embeddings to 2D with t-SNE and plotted them to inspect natural groupings
• Categorised reviews into topics using cosine similarity to topic descriptions 
• Built a similarity search that returns the 3 most semantically similar reviews for a query using cosine similarity

# RESULTS
• Embeddings stored for 958 reviews, reduced to a 2D numpy array for visualisation
• Visible clusters for themes such as fit, fabric quality and style
• Similarity search retrieved relevant reviews even without shared keywords: 'Absolutely wonderful - silky and sexy and comfortable', 'Very comfortable and versatile. got lots of compliments.', 'This is a very comfortable and sexy sleep dress, the way it drapes. i can see that the type of fabric is not suitable for out and about activities and can catch on snags, etc. very easily. once i relegated it to the nightgown category it became my favorite item to wear and lounge in.'

# TECH STACK
Python, OpenAI API (embeddings), pandas, NumPy, scikit-learn, Matplotlib
