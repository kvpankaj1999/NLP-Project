#### Cross Domain CLaim Analysis
The task here is to take a sentence and classify whether or not it is a claim. I have used two deep learning approaches for the text classification task. First approach is using a Convolutional Neural Network (CNN) with Glove pre-trained word embeddings and the second method involves the use of Recurrent Neural Network based (LSTM) for the sequential data.

I have performed extensive In-Domain experiments i.e. training and testing on the same dataset and Cross-Domain experiments which involve training on one dataset and testing on the other. I have also performed an experiment which involves training on all datasets leaving one dataset and testing on it. F1-score of the claimed class and the Macro F1 score have been calculated for the evaluation.

To overcome the problem of insufficient data, for each model, negative samples have been randomly dropped so that the ratio of the positive and the negative classes remains the same. To cover up the loss of information on dropping the data, 20 such models have been made for each classification task and during the testing of the models the average of the Macro F1 score has been calculated as the final score of the problem. This methodology has led to a good consistent
result of the F1 score of the claimed class in all the experiments made. Each model was trained on 15 iterations and 10% of the training data was kept as the unseen test data.


#### Keywords
Deep Learning, Convolutional Neural Network
(CNN), Recurrent Neural Network (RNN), LSTM,
Text Classification

#### Dataset
VG: Reed et al. (2008), http://www.aifdb.org
WD: Habernal and Gurevych (2015), https://www.informatik.tu-darmstadt.de/ukp/research_6/data/argumentation_mining_1/argument_annotated_user_generated_web_discourse/index.en.jsp
PE: Stab and Gurevych (2017), https://www.informatik.tu-darmstadt.de/ukp/research_6/data/argumentation_mining_1/argument_annotated_essays_version_2/index.en.jsp
OC: Biran and Rambow (2011a), http://www.cs.columbia.edu/~orb/code_data/persuasion_data.zip
WTP: Biran and Rambow (2011b), http://www.cs.columbia.edu/~orb/code_data/persuasion_data.zip
MT: Peldszus and Stede (2015), https://github.com/peldszus/arg-microtexts

#### References

     1. Daxenberger, Johannes & Eger, Steffen
        & Habernal, Ivan & Stab, Christian &
        Gurevych, Iryna. (2017). What is the
        Essence of a Claim? Cross-Domain
        Claim Identification.
     2. Nguyen, Son & Nguyen, Le-Minh & Tojo,
      Satoshi & Satoh, Ken & Shimazu, Akira.
      (2018). Recurrent neural network-based
      models for recognizing requisite and
      effectuation parts in legal texts. Artificial
      Intelligence and Law. 1-31.
      10.1007/s10506-018-9225-1.
