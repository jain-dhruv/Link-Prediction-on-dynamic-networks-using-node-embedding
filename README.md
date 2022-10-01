# Link-Prediction-on-dynamic-networks-using-node-embedding

Link Prediciton is a task in Social Network Analysis in which we try to predict whether a link exist between two nodes in a given graph on the basis of already existing links. There are various method to predict links, however in this repository we have node embedding technique specifically Node2Vec which is similar to Word2Vec used in Natural language processing.

In dynamic networks the links changes between the nodes with time hence it is quite complex in comparison to Static Networks. Thus, in dynamuic networks dataset timestamps are present for the already existing links.

We have divided our datasets into different snapshots and have first applied node2vec independently on each snapshot
and the obtained node representations are combined only afterwards.

After obtaining edge features using node2vec from all the snapshots except the last one, we have used these features for predicitng links in our last snapshot and have used supervised classification for obtaining predictions.

We have used three different classifiers:
1) Logistic regression
2) Random forests
3) Gradient Boosting

### Datasets

1. College Msg</br>
2. math-overflow</br>
3. fb-forum</br>
4. radoslaw-email</br>

```
datasets.zip
```
### Preprocessing
```
gae.zip
```











