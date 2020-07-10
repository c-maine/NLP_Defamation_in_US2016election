# NLP Project: Defamation in the U.S. 2016 Presidental Election

Introduction to the project:

Political Influence Campaigns by governments to influence public opinion and election outcomes in another country represent just one way in which governments have effected regime change or intervened in the affairs of another country to domestic advantage. However, with growing evidence that the world’s most powerful country (the U.S.) has been under attack more recently (especially in the 2016 U.S. presidential elections), it is unsurprising that world media attention and academic funding has increased its focus on this topic. Foreign influence is of importance because it threatens a nation’s sense of sovereignty and right to self-determination, which are core democratic values. In some cases, a power imbalance may be exploited in order to achieve change favourable to the foreign power, and this can also lead to a sense of exploitation by the receiving state. According to (Martin & Shapiro 2019), foreign influence efforts (FIE) can be categorized into 5 strategies: defamation, persuasion, polarization, shifting political agendas, and undermining institutions. This paper looks to further analyze defamation attempts by Russia through in the 2016 US elections by combining text analysis, unsupervised learning through topic modeling, and supervised learning through sentiment analysis. 

We used Twitter's Election Integrity Data Archive to access public datasets suspected of conducting malicious activity in effort to influence foreign elections. Twitter is a social media platform which enables  users  to  communicate  short statements  (a  tweet) of 140-character limit to  their audience and enables them to reach millions of individuals within seconds.  The platform is accessible to everyone through its website or mobile application. The selected dataset for this paper originates from Russia and is believed to have malicious or fake account activity. The tweets were cleaned and preprocessed to fit the needs of our model with the final version consisting of 540,953 tweets by 320 accounts. The selected time frame of the tweets was between July 1st, 2014 and October 1st, 2017.

We first used MALLET (MAchineLearning for LanguagE Toolkit) by \cite{McCallumMALLET} which is a quick topic model implementation giving a snapshot of topics in a corpus. Using MALLET, we could explore and identify the optimal number of topics given our unique dataset and verify the content was relevant to the 2016 US elections. To model defamation in particular, we created an index to measure the extent of defamation in tweets targeted to a specific person over time. We created the index by identifying key politicians relevant to our data and combining that with a defamation dictionary of negative, emotional and offensive language used in Donald Trump’s tweets. We measured defamation by comparing language similarity between a tweet and the aforementioned defamation dictionary, followed by calculating the frequency of politician references in each tweet. Our results show many defamation attempts for the politicians identified in our corpus. Hillary Clinton had the highest defamation score with tweets targeted towards her having the second highest similarity to defamatory language.

This repo is structured as follows: 

1. Data pre-processing in NLP_PreProcessing_US2016election.ipynb

2. Data exploration in 

3. Topic identification using the LDA Mallet model in LDAMallet_US2016election.ipynb


