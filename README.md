# A Dataset for Detecting Humor in Telugu Social Media Text
Increased use of online social media sites has given rise to tremendous amounts of user generated data. Social media sites have become a platform where users express and voice their opinions in a real-time environment. Social media sites such as Twitter limit the number of characters used to express a thought in a tweet, leading to increased use of creative, humorous and confusing language in order to convey the message. Due to this, automatic humor detection has become a difficult task, especially for resource-less languages such as the Dravidian languages. Humor detection has been a well studied area for resource rich languages due to the availability of rich and accurate data. In this paper, we have attempted to solve this issue by working on resource-less languages, such as, Telugu, a Dravidian language, by collecting and annotating Telugu tweets and performing automatic humor detection on the collected data. We experimented on the corpus using various transformer models such as Multilingual BERT, Multilingual DistillBERT and XLM-RoBERTa to establish a baseline classification system. We concluded that XLM-RoBERTa was the best-performing model and it achieved an F1-score of 0.82 with 81.5\% accuracy. 

If you use any source code or dataset included in this repo, please cite this paper:
```
@inproceedings{bellamkonda-etal-2022-dataset,
    title = "A Dataset for Detecting Humor in {T}elugu Social Media Text",
    author = "Bellamkonda, Sriphani  and
      Lohakare, Maithili  and
      Patel, Shaswat",
    booktitle = "Proceedings of the Second Workshop on Speech and Language Technologies for Dravidian Languages",
    month = may,
    year = "2022"
}
```
[[Paper]](https://aclanthology.org/2022.dravidianlangtech-1.2/)

# Dataset statistics

| Category  | Tweets | Words |
| ------------- | ------------- | ------------- |
| Humorous  | 458 | 5477  |
| Non-Humorous  | 1918 | 18098  |
| Other | 273 | 4213 |

The dataset contains Tweet id which can be scraped using the Twitter API. Furthermore, the labels are as follows: 
1. 0 indicating non-humourous text
2. 1 indicating humourous text
3. n/N indicating facts or tweet with images/video.

We have provided the train and test dataset in the data folder. The training data contains 732 examples while the test data contains 184 examples.
# Results

| Model  | Accuracy | F1-score |
| ------------- | ------------- | ------------- |
| Multilingual BERT | 81.5 | 0.81 |
| Multilingual DistilBERT | 73.4 | 0.73 |
| XLM-RoBERTa | 81.5 | 0.82 |
