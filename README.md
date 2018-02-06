# Personalized Medicine Redefining Cancer Treatment 

# Statement:-
    To classify every single genetic mutation based on evidence from text-based clinical literature using Machine Learning. 

# Problem Description:-
    A lot has been said during the past several years about how precision medicine and, more concretely, how genetic testing is 
    going to disrupt the way diseases like cancer are treated. But this is only partially happening due to the huge amount of 
    manual work still required. 
    Once sequenced, a cancer tumour can have thousands of genetic mutations. But the challenge is distinguishing the mutations 
    that contribute to tumour growth (drivers) from the neutral mutations (passengers).  
    Currently this interpretation of genetic mutations is being done manually. This is a very time- consuming task where a 
    clinical pathologist has to manually review and classify every single genetic mutation based on evidence from text-based 
    clinical literature. 
    For this competition MSKCC is making available an expert-annotated knowledge base where world-class researchers and 
    oncologists have manually annotated thousands of mutations .We need your help to develop a Machine Learning algorithm that, 
    using this knowledge base as a baseline, automatically classifies genetic variations.

    This project was introduced as one of kaggle problems.So firstly they had provided us with the training data only, so to 
    test my models i just did 70-30 split for train and text data.So whole of my project is modeled on the basis of train data 
    only.As the data was imbalanced so i had to do split on every class label.
    In this project i have tried to do full exploratory data analysis on gene,variaion and text provided as well as i tried to 
    implement some of the machine learning algorithms after preprocessing text data.The maximum accuracy i got is 43%.
 

# Data:  
    The data provided could be found on kaggle link:
    <a href="https://www.kaggle.com/c/msk-redefining-cancer-treatment#evaluation">Click here</a> to get the dataset.<br />
    
    1. training_variants - a comma separated file containing the description of the genetic mutations used for training. Fields 
    are ID (the id of the row used to link the mutation to the clinical evidence), Gene (the gene where this genetic mutation is 
    located), Variation (the amino acid change for this mutations), Class (1-9 the class this genetic mutation has been 
    classified on) 
    2. training_text - a double pipe (||) delimited file that contains the clinical evidence (text) used to classify genetic          
    mutations. Fields are ID (the id of the row used to link the clinical evidence to the genetic mutation), Text (the clinical 
    evidence used to classify the genetic mutation) 
    3. test_variants - a comma separated file containing the description of the genetic mutations used for training. Fields are 
    ID (the id of the row used to link the mutation to the clinical evidence), Gene (the gene where this genetic mutation is 
    located), Variation (the amino acid change for this mutations) 
    4.test_text - a double pipe (||) delimited file that contains the clinical evidence (text) used to classify genetic    
    mutations. Fields are ID (the id of the row used to link the clinical evidence to the genetic mutation), Text (the clinical 
    evidence used to classify the genetic mutation) 
    5. submissionSample - a sample submission file in the correct format  
  
# Data Type:-
    double (||) pipe delimited and csv files. 
    training_variants.csv(Id , Gene, Variations, Class)
    training_text(ID, Text) 
    test_variants.csv(Id , Gene, Variations) 
    test_text (ID, Text) 

Data Size:- 159 MB 

# Paper:- 
    1. The Path to Personalized Medicine 
    http://www.nejm.org/doi/full/10.1056/nejmp1006304#t=article  

# Useful Links :- 
    1. Kaggle :- https://www.kaggle.com/c/msk-redefining-cancer-treatment 
    2. http://onlinelibrary.wiley.com/doi/10.1038/clpt.2012.237/full 
    3. https://www.cancer.org/latest-news/personalized-medicine-redefining-cancer-and-its- treatment.html  

# Modelling:  
    Pre-processing of the data for both test and train using different methods(w2vec,Tfidf or bag of words).
    models used:
    1.Decision tree classifier
    2.Logistic Regression 
    3.Multinomial Naive Baye's
    4.Linear Svc
    5.RBF SVM
    6.tfidf + Count Vectorizer + Linear SVC
    7.K_Nearest_Neighbours
