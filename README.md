# Detecting-SMS-Spam-with-Tensorflow

## Motivation
A neural network trained on SMS messages designed to classify SMS spam. 

The SMS Spam Collection is a public set of 5,574 SMS labeled messages that have been collected for mobile phone spam research [1].

The algorithm was able to learn the message vocabulary and idf, then return the term-document matrix through the sklearn TfidfVectorizer class. The binary label was one hot encoded with the sklearn LabelEncoder class. 

## Neural Network Topology and Results Summary

The binary-crossentropy loss function was leveraged along with the Nadam optimizer for this classification problem.

![model](https://user-images.githubusercontent.com/48378196/96961401-4be81500-1550-11eb-9cd2-4e0f682c3b56.png)

After 35 epochs the binary and validation classifiers reaches 98% and 97 accuracy, respectively, in predicting SMS spam. 

![spam](https://user-images.githubusercontent.com/48378196/98815483-5294e880-247b-11eb-9d65-e3c53cca3cf3.png)

## License
[MIT](https://choosealicense.com/licenses/mit/) 

## References
[1] Almeida, T.A., Gómez Hidalgo, J.M., Silva, T.P.  Towards SMS Spam Filtering: Results under a New Dataset.   International Journal of Information Security Science (IJISS), 2(1), 1-18, 2013. [Invited paper
