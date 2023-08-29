# Voice of Customer with NLP 
- The Voice of the Customer holds valuable insights that, when comprehended and acted upon, result in enhanced customer satisfaction and revenue growth. Gartner's research indicates that gathering customer feedback can boost cross-selling and upselling success rates by 15-20%, underscoring the potential benefits of leveraging customer insights for strategic business actions.

- In the evolving landscape, quicker customer feedback enables swift trend spotting and tailored offerings. Yet, lacking proper tools, this influx of unstructured data can become a bewildering disarray, impeding valuable insights for brands.
  
- A substantial portion of consumer data, including reviews, social media content, and search queries, is expressed through natural language. Natural Language Processing (NLP) encompasses a set of methods for analyzing and representing this text that occurs organically.
  
- In the following discussion, we'll explore natural language processing techniques and real-world applications that brands employ to gain deeper insights into the digital consumer's voice.

# Use Case of Voice of Customer : SALA Samui Chaweng Beach Resort     
***Step to do Voice of Customer (VOC) with NLP***    
- Data processing/analyzing
- Data cleansing
- Data augmentation
- Feature extraction.
- Data point for plotting/reporting


***Basic linguistic features***
**▪ Language identification**
consists in detecting the language used in a text. It allows defining the models to be applied to carry out the other activities.
**▪ Separation of sentences**    
(also called sentence boundary disambiguation), words, or groups of words. Many NLP tasks need to work at the sentence or word level, hence the importance of this processing. This activity is therefore essential in a text processing chain.    
**▪ Word tokenization**    
is the process of splitting a large sample of text into words. This is a requirement in natural language processing tasks where each word needs to be captured and subjected to further analysis like classifying and counting them for a particular sentiment etc.     
**▪ Stemming and lemmatization**    
Stemming consists of extracting the root of the word. Lemmatization allows reducing a word to its canonical form (the lemma). It is also called the “dictionary” form.    
**▪ Word embedding and sentence embedding**    
Word embedding and sentence embedding, and by extension of paragraphs and documents, transform the element into a vector of numbers. Vectorization is currently a fundamental operation to perform similarity searches, clustering, classifications, etc.    



## Comment from Tripadvisor     
Sampling comment from trip advisor of SALA Samui Chaweng Beach Resort for 13 comments which the comment shown below:    
![CDP Flow](https://github.com/Pinnun/MADT8101-Seminar-in-Advanced-Analytic/blob/58ad84a6a6c8d6d30c00789ccad5d473a29b89b4/6%20VOC/Raw%20Data/TripadvirsorReview1.png)
## Topic Modeling with LDA     
![CDP Flow](https://github.com/Pinnun/MADT8101-Seminar-in-Advanced-Analytic/blob/58ad84a6a6c8d6d30c00789ccad5d473a29b89b4/6%20VOC/Raw%20Data/PCA%20Result.png
)
Group 1 Facilities
![CDP Flow](https://github.com/Pinnun/MADT8101-Seminar-in-Advanced-Analytic/blob/58ad84a6a6c8d6d30c00789ccad5d473a29b89b4/6%20VOC/Raw%20Data/Group1.png)
Group 2 Design
![CDP Flow](https://github.com/Pinnun/MADT8101-Seminar-in-Advanced-Analytic/blob/58ad84a6a6c8d6d30c00789ccad5d473a29b89b4/6%20VOC/Raw%20Data/Group2.png
)
Group 3 Ambiance
![CDP Flow](https://github.com/Pinnun/MADT8101-Seminar-in-Advanced-Analytic/blob/58ad84a6a6c8d6d30c00789ccad5d473a29b89b4/6%20VOC/Raw%20Data/Group3.png)
Python Code:
[VOC Python](https://github.com/Pinnun/MADT8101-Seminar-in-Advanced-Analytic/blob/d3d9c55dc701d63abdc7d9a5ab8e2d0efd47f741/6%20VOC/Raw%20Data/Python/Sala%20Samui.ipynb)
## Result for Topic Medeling with LDA     
![CDP Flow](https://github.com/Pinnun/MADT8101-Seminar-in-Advanced-Analytic/blob/58ad84a6a6c8d6d30c00789ccad5d473a29b89b4/6%20VOC/Raw%20Data/Result1.png)
##  VOC Extracting Information     
![CDP Flow](https://github.com/Pinnun/MADT8101-Seminar-in-Advanced-Analytic/blob/58ad84a6a6c8d6d30c00789ccad5d473a29b89b4/6%20VOC/Raw%20Data/Extracting%20Information.png)
## Another use case of VOC with NLP
Brands can leverage natural language processing techniques in several ways. For instance, a fast food restaurant could employ area charts to discern market trends, enabling them to enhance services in specific domains. Evaluating sentiment scores, topics, and keywords extracted from customer feedback can aid in understanding newly launched products or stores. Additionally, predefined response templates, guided by dominant topics predicted by VoCA models, can enable businesses to craft smart and relevant replies to reviews.
