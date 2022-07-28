# VASP-Recommender-System
A Tensor-flow implementation of a Recommender System which takes in a sparse user-item rating matrix to generate new entries using which items can be recommended to users.


It is inspired by the model described in the publication: 
[Deep Variational Autoencoder with Shallow Parallel Path for Top-N Recommendation (VASP) ](https://www.researchgate.net/publication/354505790_Deep_Variational_Autoencoder_with_Shallow_Parallel_Path_for_Top-N_Recommendation_VASP)
It is recommended to read the above paper for better unerstanding of the implementation. 
Note: A closed-form solution of EASE is implemented here instead of the Neural EASE model. 


## Implementation Description:
### Input:
A sparse matrix containing the ratings of movies rated by different users obtained from [MovieLens100k](https://www.kaggle.com/datasets/rajmehra03/movielens100k?select=ratings.csv).
### Output:
A Hadamard product of the matrix generated using the EASE Model and the matrix generated using a Varational Auto-Encoder. This matrix contains new user-movie rating entries which is used to provide new movie recommendations to the users.
