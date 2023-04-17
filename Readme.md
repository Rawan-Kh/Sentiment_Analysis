## Twitter sentiment analysis of airlines:
In this notebook, we are going to explore different sentiment analysis procedures but we will not train any new one. 
### Here are the contents of this notebook:
(1) Data analysis and cleaning for airline data<br/>
(2) sentiment analysis using NLTK<br/>
(3) sentiment analysis using textblob<br/>
(4) sentiment analysis using huggingface<br/>
(5) sentiment analysis using flair<br/>

## Conclusion:
In this notebook, we preprocessed a airline tweet data set and then used both nltk ( VADER based pretrained system) and textblob to detect, and generate the scores for sentiments for the tweets. We did a bit of superficial observation of the performance of both the systems as well. In both cases, we saw that very implicitly meant negative cases are missed by the models; and hints at the importance of custom sentiment model training.<br/>
We also tried out a number of pretrained models from huggingface for sentiment analysis and the vanilla models didn't function well, while models specifically trained for sentiment performed much better.<br/>
### percentage-wise model comparison:
The NLTK, textblob performed at 50% around accuracy, and while facebook's bart model seemed to be unfit for the downstream task of sentiment analysis, other two models such as the default huggingface model for sentiment analysis performed at 89% accuracy for positive/negative sentiment classification and the cardiffnlp's twitter data based roberta model performed at 70% accuracy for the 3 class classification.<br/>


### Acknowledgements:
I would like to thank SHYAMBHU MUKHERJEE for the great Insights.
