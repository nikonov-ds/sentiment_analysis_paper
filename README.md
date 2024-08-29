## INITIAL INVESTIGATION OF THE SENTIMENT ANALYSIS SIMILARITIES AND CONSISTENCIES IN ENGLISH AND CHINESE

This is the code for my Master's Dissertation and the conference paper.

**ABSTRACT**


With the advancement of the Internet and the trendiness of social media platforms, people have started sharing their opinions on any matter more openly. It enables businesses to monitor customer satisfaction with their products or services. Sentiment analysis is an approach to natural language processing that allows them to do just that. With most online activity being in English, the field of English sentiment analysis has been developing quite rapidly. In contrast, sentiment analysis in other languages and the effect of machine translation on it remains far less explored. This master’s dissertation proposes a CNN-based sentiment analysis model for short messages written in Chinese built using SpaCy, a Python library for natural language processing. It also attempts an initial investigation of the sentiment analysis similarities and consistencies in English and Chinese. The proposed method of Chinese text classification achieved an F1-score of 0.554, while the chosen lexicon-based approach to English sentiment analysis on translated comments performed with an F1-score of 0.419.


**CONCLUSION**

This research aimed to conduct an initial evaluation of the accuracy of Google Translate in conveying the sentiment of short comments written in Chinese from a popular Chinese microblogging website Weibo when translated into English. With TextBlob being the tool for predicting the sentiment of the translated comments, the aim of the research was achieved.

In the course of the research, an ensemble of an n-gram bag-of-words and a convolutional neural network built upon a Tok2Vec layer with a layer-normalized maxout activation function and attention was trained. The model was configured and implemented using SpaCy, a natural language processing library for Python, and its TextCategorizer component. Although the proposed method achieved a macro F1-score of only 0.554, it performed better on the original data than TextBlob on the translation of the said data.

**CONTRIBUTIONS**

* This is the first research done on the data collected by Wei and Zhang and described in their paper (Wei and Zhang, 2024) that the author of this dissertation is aware of.
* It sets the baseline for the future work done on this dataset.
* Although the proposed model for Chinese has a macro F1-score of 0.554, the precision for the POSITIVE label is 0.736, meaning that a Chinese comment labeled POSITIVE by this model has a 73.6% chance of truly being POSITIVE.
* The proposed model proved to be more reliable in terms of correctly predicting the sentiment of a Chinese comment than TextBlob in predicting the sentiment of its English translation. Although the results are not state-of-the-art, the model can be used by businesses to assess the sentiment of short Chinese comments instead of translating them via Google Translate and using TextBlob.
