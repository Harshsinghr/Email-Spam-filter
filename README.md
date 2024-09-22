# Email Spam Filter

## Introduction

In this project, we will design an e-mail spam ﬁlter using a Naïve Bayes and SVM based classiﬁcation on the ling-spam dataset.

## Dataset

The ling-spam corpus contains e-mails from the Linguist mailing list categorized as either legitimate or spam emails. The corpus is divided into four sub-folders that contain the same emails that are pre-processed with/without lemmatization and with/without stop-word removal. The e-mails in each sub-folder partitioned into 10 "folds".

In this project, we will use the ﬁrst 9 folds from the ling-spam corpus (lemm_stop folder, with both lemmatization and stop-word enabled) as training data, and the 10th fold as test data.

Download the whole ling-spam dataset from this [link](http://www.aueb.gr/users/ion/data/lingspam_public.tar.gz ).

Each one of the 10 subdirectories contains both spam and legitimate messages, one message in each file. Files whose names have the form spmsg*.txt are spam messages. All other files are legitimate messages.

## Feature Selection

Feature selection is performed using the information gain (IG) metric. From the training data, select the top-N features for N = {10, 100, 1000}. Note that feature selection based on the IG metric only accounts for the occurrence of (and not frequency with which terms appear) in the dataset.

## Classifiers

In the Jupyter notebook `email_spam_filter.ipynb`, 5 different classifiers are implemented.

Here is a list of email spam filters:

*  Naive Bayes Classifier
  * Bernoulli NB classiﬁer with binary features
  * Multinomial NB with binary features
  * Multinomial NB with term frequency (TF) features
* SVM based Classifier
* Adversarial Classification

For the last but not least classifier, which is "Adversarial Classifier", is an approach to update NB based e-mail spam ﬁlters in response to attacks that try to evade a basic NB ﬁlter. It is inspired from [paper](https://dl.acm.org/doi/10.1145/1014052.1014066).

## Contributing

Contributions are welcome! If you would like to contribute to this project, please follow these steps:

1. Fork the repository
2. Create a new branch (git checkout -b feature/YourFeature)
3. Make your changes
4. Commit your changes (git commit -m 'Add some feature')
5. Push to the branch (git push origin feature/YourFeature)
6. Open a Pull Request

## Guidelines for Contributions
- Ensure your code is well-documented.
- Follow consistent coding styles.
- Include tests for new features.
- Respect the repository's code of conduct.

## Contact
For any queries or to connect, feel free to reach out:

- Email: 31608csai@gmail.com
- LinkedIn: [https://www.linkedin.com/in/harsh-singh27/](https://www.linkedin.com/in/harsh-singh27/)

I welcome any questions or discussions related to this project!

## License
This project is licensed under the MIT License. See the LICENSE file for details.


Thank you for visiting the Email-Span-filter repository! Happy coding!🎉
