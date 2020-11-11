# Detecting-SMS-Spam-with-Tensorflow

## Motivation
A binary classification machine learning algorithm for detecting SMS spam. 

A collection of 425 SMS spam messages was manually extracted from the Grumbletext Web site. This is a UK forum in which cell phone users make public claims about SMS spam messages, most of them without reporting the very spam message received. 

A subset of 3,375 SMS randomly chosen ham messages of the NUS SMS Corpus (NSC), which is a dataset of about 10,000 legitimate messages collected for research at the Department of Computer Science at the National University of Singapore.

Also incorporated is the SMS Spam Corpus, which has 1,002 SMS ham messages (genuine) and 322 spam messages [1].

The algorithm was able to learn the message vocabulary and return the term-document matrix through the sklearn TfidfVectorizer class. The binary label was one hot encoded with the sklearn LabelEncoder class. 

## Neural Network Topology and Results Summary

The binary-crossentropy loss function was leveraged along with the Nadam optimizer for this classification problem.

![model](https://user-images.githubusercontent.com/48378196/96961401-4be81500-1550-11eb-9cd2-4e0f682c3b56.png)

After 35 epochs the binary and validation classifiers reaches 98% and 97 accuracy, respectively, in predicting SMS spam. 

![spam](https://user-images.githubusercontent.com/48378196/98815483-5294e880-247b-11eb-9d65-e3c53cca3cf3.png)

Although impressive, considering the relatively small data set of 120 instances, these expectations should be judiciously adjusted when applied to larger data sets.


## License
[MIT](https://choosealicense.com/licenses/mit/) 

## References
[1] Almeida, T.A., Gómez Hidalgo, J.M., Silva, T.P.  Towards SMS Spam Filtering: Results under a New Dataset.   International Journal of Information Security Science (IJISS), 2(1), 1-18, 2013. [Invited paper
