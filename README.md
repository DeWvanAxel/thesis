# thesis
The classification of municipality documents

# Finished at 4-23
1. Loading in new data from zoek.officielebekendmakingen.nl
2. Loading in data from api.openraadsinformatie.nl
3. Standard pre-processing of the data 
4. Lay-out to create correct overview of the data
5. Import of pre-trained Word2Vec embeddings
6. Implementation of Multinomial Naive Bayes, Stochastic Gradient Descend, Random Forest, Logistic Regression
7. Implementation of CNN
a. Standard deep implementation with constant filter size
b. Deep implementatation with a mix of filter sizes
c. Cutting up sentences into smaller parts and classifying each individual part, then aggregating that into one prediction. This can be combined with a and b
8. Set of evaluation criteria, consisting of recall, accuracy, precision, F1 and possibility to show performance during epoch and amount of training data.
9. Written introduction
10. classified handfull of data within test set of openraadsinformatie

# Short term goals
1. Loading in enough data, preferably from 2000 untill now. 9000 is just not enough.
2. Retraining of all baselines with parameter optimalization
3. Retraining of CNN's without parameter optimalization
4. Writing literature review and methodology

# Longer term goals
1. Other implementation of CNNs such as par2vec and pooling layers for long sentences
2. Parameter optimalization, such as filter sizes, aggregation methods, activation functions, loss functions
3. Own Word2Vec implementation with specialized corpus, and checks how that contributes to metrics
4. Contribute to OpenState implementation
5. check performance on openraadsinformatie-set + perhaps categorize when to try predicting
6. Writing results, discussion and conclusion



# Timeline
| Week         | Finish                                                                                                             |
|--------------|--------------------------------------------------------------------------------------------------------------------|
| 23/4-29/4    | Load in all data, create overview of that data, and save it in pre-processed, final form                           |
| 30/4-6/5     | Re-test baselines with all data, write that down in tables, never touch them again                                 |
|              | Re-test CNNs and re-evaluate what priorities and goals are, is beating baselines possible?                         |
|              | Writing literature review and methodology                                                                          |
| 7/5-13/5     | Par2vec and pre-pooling as solutions for long documents                                                            |
| 14/5-20/5    | First test of par2vec and pre-pooling                                                                              |
|              | Overview of results, a indication of where most improvements can be achieved and planning for most promising tests | 
|              | Mid-term progress and evaluation report                                                                            |
| 21/5-27/5    | Testing and changing small pieces                                                                                  |
| 28/5-3/6     | Testing and changing small pieces                                                                                  |
|              | Implement word2Vec on most promising algorithms                                                                    |
| 4/6-10/6     | Final checks on test set of municipalities                                                                         |
|              | Assist with final implementation for OSF                                                                           |
|              | Results section                                                                                                    |
| 11/6-17/6    | Discussion and future work section                                                                                 |
|              | Spell-check, lay-out and abstract section                                                                          |
| 18/6-24/6    | Thesis                                                                                                             |
| 25/6-1/7     | Defence of thesis                                                                                                  |
  
