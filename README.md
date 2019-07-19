# Review Classifier and Spam Identifier 

This is a project that uses Natural language processing techniques to classify a given review as positive or negative. Further, this classifier is also capable of identifying spam reviews that often occur in the real world. 

The classifier is built using a three layer deep neural network using barebones tensorflow. 
Activations functions : tanh and relu 
First layer - The numpy array of all tokenized words in the review 
Second layer(hidden) - Dimensionality reduced to 40, randomly drop 50% of the weights to avoid over fitting 
Third layer(hidden) - Dimensions down to 10 
Output layer - Positive, negative/ Spam, not spam 

## Visualization 
The dataset is visually inspected by using some random random words to check their significance in classification 
For example - noun words like 'furniture' or 'location' do not really help in deciding whether a review is positive/negative or spam/real. It can further observed that adjectives play a more significant role in distinguising positive/negative and spam/not spam. 

To coveniently plot, we bring down the large number of features down to 2 features using tsne. 
The resulting 2D features are plotted against a 2D graph. The t-SNE plot is uploaded as tsne_embeds.pdf 

### Observations from the t-SNE plot
- The dots in color blue: positive and orange:  negative
- The other dots in green->location and red->furniture. 
- We can observe that a clear distinction exists between the positive and negative dots. 
- The dots that depict location and furniture are mixed and scattered -> these features do not help towards classification. 

![GitHub Logo](/tsne_embeds.pdf)
Format: ![Alt Text](url)
