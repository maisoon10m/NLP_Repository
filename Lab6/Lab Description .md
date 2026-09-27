Lab 6: Deep Learning for NLP
Aim
Classify Yelp restaurant reviews as negative (0) or positive (1) using neural networks. Compare two ways of representing text: TF-IDF and Word2Vec.
Dataset
The dataset contains 1,000 reviews. Each review has a text field and a sentiment label. The notebook uses 80% of the reviews for training and 20% for testing.
Lab workflow
1. Load and preprocess the reviews. Convert text to lowercase, remove punctuation and special characters, and remove extra spaces.
2. Build the TF-IDF example. Convert reviews into TF-IDF feature vectors, then train a PyTorch neural network to predict their sentiment.
3. Task 1 — Represent reviews with Word2Vec. Tokenize the reviews, train Word2Vec on the training reviews (vector_size=200, window=5, min_count=1, sg=1), and average the word vectors to produce one 200-number vector per review. Convert these vectors into PyTorch tensors.
4. Task 2 — Train a second neural network. Use the Word2Vec review vectors as input. The network follows 200 → 128 → 64 → 32 → 1, with ReLU after each hidden layer. Train for 15 epochs using BCEWithLogitsLoss and Adam with a learning rate of 0.001.
5. Evaluate the models. Use the test reviews to calculate classification accuracy. The TF-IDF example also displays a classification report and confusion matrix.
Key idea
TF-IDF and Word2Vec turn text into numbers in different ways. The neural network takes those numbers as input and learns to predict the review label. Test accuracy measures how often its predictions are correct on reviews held aside during training
